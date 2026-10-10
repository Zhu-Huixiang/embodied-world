# Causal World Modeling for Robot Control

**LingBot-VA** · RSS 2026 · 本版排名 82 · 综合分 **82.3 / 100**

[解读导读](../../../library/lingbot-va.md) · [视频动作模型与视觉推理](../../../paper-map/README.md#track-video-action) · [RSS集锦](../../../venues/RSS/README.md)

[原文](https://www.roboticsproceedings.org/rss22/p016.html) · [PDF](https://www.roboticsproceedings.org/rss22/p016.pdf) · [阅读卡片](../../../library/lingbot-va.md)

论文出处：[**Lin Li / Qihang Zhang 等3位**](../../origins/papers/lingbot-va.md)<br>[蚂蚁灵波具身研究团队 / 香港科技大学 · 另6个机构](../../origins/papers/lingbot-va.md)

## 机制简析

因果视频VAE把观测压到48通道latent；Wan2.2-5B视频stream和动作stream经MoT联合处理，chunk间因果、chunk内并行。T5指令条件、真实obs/action写回KV cache、noisy-latent augmentation支持视频部分去噪后解动作；统一双臂30维动作，5.3B总参数。

带着这个问题读：视频预测具体给动作带来什么，真实反馈怎样写回KV历史，又怎样少去噪而保住控制质量？

初读判断：联合未来预测与动作推断、持久历史和部分去噪控制有可验证机制。RSS版新增action-only/causal ablation、RoboTwin与LIBERO、6项实机 paired trials，证据增强。历史策略在进度被逆转时会退化、视频推理成本高，部分baseline来自他论文，正式主表和消融数值须按定位区别。开源部署、posttrain与权重支持复用，完全重训算力成本限制复用分。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 88 | 20% |
| 实验与证据 | 87 | 20% |
| 学术影响 | 13.7 | 10% |
| 近期关注 | 82.1 | 5% |
| 复用价值 | 86 | 8% |
| 阅读价值 | 92 | 7% |

刊会依据：[RSS 2026](../../../venues/RSS/README.md)，正式出处见[出版/原文记录](https://www.roboticsproceedings.org/rss22/p016.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：RSS正式原文机制与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：Causal World Modeling for Robot Control。累计被引 **2**，2025–2026 被引 **2**；快照：2026-10-10T11:42:48+08:00。

[指标记录](https://api.openalex.org/works/W7126180855) · [文献计量条目](https://openalex.org/W7126180855)

### 影响与关注的计算依据

- **学术影响 13.7**：身份匹配的累计引用C=2，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W7126180855)
- **近期关注 82.1**：近期窗口内创建的专属论文仓库，快照star=1927；按10000上限对数压缩。 [依据1](https://api.github.com/repos/Robbyant/lingbot-va) · [依据2](https://raw.githubusercontent.com/Robbyant/lingbot-va/main/README.md)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/Robbyant/lingbot-va) | GitHub Star 1927；GitHub Watch订阅 12；GitHub Fork 187 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2601.21998) | HF 论文累计点赞 32 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/robbyant/lingbot-va-base) | HF 最近30天下载 0；HF 仓库累计点赞 33 | 单篇论文的作者发布资产；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
