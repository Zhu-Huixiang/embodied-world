# Causal World Modeling for Robot Control

**解读导读** · RSS 2026 · [视频动作模型与视觉推理](../paper-map/README.md#track-video-action)

研究范围：因果视频动作生成、持久历史与双臂闭环操作。

[原文入口](https://www.roboticsproceedings.org/rss22/p016.html) · [原文 PDF](https://www.roboticsproceedings.org/rss22/p016.pdf) · [作者项目 / 代码入口](https://technology.robbyant.com/lingbot-va) · [作者与团队](../leaderboard/origins/papers/lingbot-va.md)

RSS2026正式版；官方HTML摘要保留CauVA旧称，PDF及作者repo为LingBot-VA，同一原研究。RSS主表TableI为92.0/91.1；消融TableIII的baseline92.93属该表条件；不与arxivv2的92.93/91.55混作同一结果。

## 先看它做了什么

因果视频VAE把观测压到48通道latent；Wan2.2-5B视频stream和动作stream经MoT联合处理，chunk间因果、chunk内并行。T5指令条件、真实obs/action写回KV cache、noisy-latent augmentation支持视频部分去噪后解动作；统一双臂30维动作，5.3B总参数。

## 带着什么问题读

**视频预测具体给动作带来什么，真实反馈怎样写回KV历史，又怎样少去噪而保住控制质量？**

## 为什么值得继续读

现有候选升级正式RSS身份，有视频/因果/去噪关键消融、两种仿真基准和六项实机任务，可精确解释世界模型进入控制的收益与成本。

证据入口：压缩video latent z∈R^(N×48)，MoT双stream；跨chunk因果、chunk内双向并行；视频Wan2.2-5B和小hidden动作stream，总5.3B。动作双臂30维。推理video3步到s=0.6，action10步到s=1.0。（§III-A/B/C and Fig2; §IV-B）；50项RoboTwin任务，2500clean+25000randomized demos；video12.5Hz，action50Hz；LingBot-VA92.0%E/91.1%H vs Motus88.7/87.0及π0.5 82.7/76.8。X-VLA/Motus为引用结果，π0.5用官方JAX复现；不同预训练源和实现不应当作全匹配协议。（§V-B / TableI）；LIBERO四suite，各10任务×50demos；3random seeds×500trials per suite；overall98.5%，π0.5(JAX)96.9%，X-VLA98.1%。（§V-B / TableII）

具身关联：因果视频动作生成、持久历史与双臂闭环操作；视频预测具体给动作带来什么，真实反馈怎样写回KV历史，又怎样少去噪而保住控制质量？

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/lingbot-va/README.md) · [RSS集锦](../venues/RSS/README.md) · [地图方向](../paper-map/README.md#track-video-action) · [首页](../README.md)

元数据核对：2026-10-10。
