# EgoScale: Scaling Dexterous Manipulation with Diverse Egocentric Human Data

**EgoScale** · arXiv 2026 · 本版排名 106 · 综合分 **47.3 / 100**

[原文](https://arxiv.org/abs/2602.16710) · [PDF](https://arxiv.org/pdf/2602.16710v1) · [阅读卡片](../../../library/egoscale.md)

## 机制简析

从第一视角human videos提取相对SE(3)腕部轨迹与重定向22DoF手关节，pretrain flow-based VLA；少量paired human/robot play midtraining对齐视觉和motor接口，再任务posttrain。统一腕部action、embodiment-specific hand/state adapters迁移至G1 7DoF手，下肢独立Homie。

带着这个问题读：人类视频怎样变成机器人可学的手腕和手指动作，为什么大量预训练之后还要一小段人机对齐数据？

初读判断：动作级human supervision、规模规律与aligned transfer组合有价值。五项实机、1k–20k小时五档规模、表示/两阶段消融和跨手型证据较丰富，但有限seed/trials、专有大数据与未全面开源、one-shot附加human supervision限制证据和复用分；R²是五个规模点内fit，不预测全域能力。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 0 | 30% |
| 创新性 | 89 | 20% |
| 实验与证据 | 84 | 20% |
| 学术影响 | 0.0 | 10% |
| 近期关注 | 0.0 | 5% |
| 复用价值 | 78 | 8% |
| 阅读价值 | 92 | 7% |

发表与刊会：预印本公开，正式发表贡献记0；创新与实验单独计分。


编辑深度：原文机制与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：EgoScale: Scaling Dexterous Manipulation with Diverse Egocentric Human Data。累计被引 0，2025–2026 被引 0；快照：2026-10-10T11:42:48+08:00。

[指标记录](https://api.openalex.org/works/W7130590664) · [文献计量条目](https://openalex.org/W7130590664)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
