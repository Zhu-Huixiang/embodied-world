# V-JEPA 2: Self-Supervised Video Models Enable Understanding, Prediction and Planning

**解读导读** · arXiv 2025 · [世界模型与模型强化学习](../paper-map/README.md#track-world-model)

研究范围：视频潜世界模型；动作条件规划与实机操作。

[原文入口](https://arxiv.org/abs/2506.09985) · [原文 PDF](https://arxiv.org/pdf/2506.09985) · [作者项目 / 代码入口](https://ai.meta.com/vjepa/)

官方代码 BibTeX 仍为 arXiv preprint；精选预印本观察项，不进入正式刊会队列。

## 先看它做了什么

masked video encoder/EMA目标先学表征；冻结编码器后训300M block-causal 动作 predictor，自回归预测未来 latent；MPC 最小化目标图 latent L1。

## 带着什么问题读

**先看无动作标签视频，再给少量机器人交互，潜空间怎样变成 Franka 规划器？**

## 为什么值得继续读

视频表征直接接动作条件预测与真实机器人 MPC；实验基线、条件和开放实现可读，按精选预印本收录。

证据入口：62小时机器人日志仍有动作输入，unlabeled指无人工语义标签；真实Franka目标图控制。77.3 SSv2 /39.7 EPIC是视频指标。（Sec.4.1/4.2与机器人表）

具身关联：视频潜世界模型；动作条件规划与实机操作；先看无动作标签视频，再给少量机器人交互，潜空间怎样变成 Franka 规划器？

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/vjepa2/README.md) · [arXiv集锦](../arxiv/README.md#paper-vjepa2) · [地图方向](../paper-map/README.md#track-world-model) · [首页](../README.md)

元数据核对：2026-10-10。
