# Cosmos Policy: Fine-Tuning Video Models for Visuomotor Control and Planning

**Cosmos Policy** · ICLR 2026 · 本版排名 100 · 综合分 **75.8 / 100**

[解读导读](../../../library/cosmos-policy.md) · [世界动作模型](../../../paper-map/README.md#track-world-action-model) · [ICLR集锦](../../../venues/ICLR/README.md)

[原文](https://openreview.net/forum?id=wPEIStHxYH) · [PDF](https://arxiv.org/pdf/2601.16163) · [阅读卡片](../../../library/cosmos-policy.md)

## 机制简析

微调视频基础模型，把动作、未来视觉状态和规划信号放进共同生成过程。

带着这个问题读：视频生成序列怎样容纳动作、未来状态与规划信号？

初读判断：视频先验到控制的接口值得看；精读需追训练条件和规划/策略消融。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 89 | 20% |
| 实验与证据 | 82 | 20% |
| 学术影响 | 0.0 | 10% |
| 近期关注 | 0.0 | 5% |
| 复用价值 | 82 | 8% |
| 阅读价值 | 93 | 7% |

刊会依据：[ICLR 2026](../../../venues/ICLR/README.md)，正式出处见[出版/原文记录](https://openreview.net/forum?id=wPEIStHxYH)；采用2026-10-10刊会快照。


编辑深度：选题初读；评分记录：2026-10-10。

计量版本：作者预印本；OpenAlex题目：Cosmos Policy: Fine-Tuning Video Models for Visuomotor Control and Planning。累计被引 0，2025–2026 被引 0；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W7125496427) · [文献计量条目](https://openalex.org/W7125496427)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
