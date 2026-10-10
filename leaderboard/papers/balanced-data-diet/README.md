# A Balanced Data Diet: Addressing the Exploration Bottleneck in Mega-Scale RL for Robot Control

**Balanced Data Diet** · arXiv 2026 · 本版排名 113 · 综合分 **44.1 / 100**

[原文](https://arxiv.org/abs/2610.12465v1) · [PDF](https://arxiv.org/pdf/2610.12465v1) · [阅读卡片](../../../library/balanced-data-diet.md)

## 机制简析

Success Guided Sampling 根据当前成功率把重置分布推向能力边缘，减少超简单或暂时学不会的采样，再蒸馏视觉操作策略转实机。

带着这个问题读：并行环境堆到很大以后，为什么探索还会卡住？

初读判断：华盛顿大学/英伟达署名；跨地形和接触操作的明确探索问题，需核对采样公平性和训练预算。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 0 | 30% |
| 创新性 | 85 | 20% |
| 实验与证据 | 77 | 20% |
| 学术影响 | 0 | 10% |
| 近期关注 | 0 | 5% |
| 复用价值 | 68 | 8% |
| 阅读价值 | 89 | 7% |

发表与刊会：预印本公开，正式发表贡献记0；创新与实验单独计分。


编辑深度：选题初读；评分记录：2026-10-10。

影响与关注采用独立证据评分：

- **学术影响 0**：本次2026-10-10补查范围内，独立采用证据仍在积累；按证据量表起点计0分。原文方法与作者实验分别进入创新、证据轴。 [依据1](https://arxiv.org/abs/2610.12465v1) · [依据2](https://github.com/Zhu-Huixiang/embodied-world/blob/main/leaderboard/selection-2026-10-10.md)
- **近期关注 0**：本次2026-10-10补查范围内，2025–2026的独立采用证据仍在积累；按证据量表起点计0分。原文方法与作者实验分别进入创新、证据轴。 [依据1](https://arxiv.org/abs/2610.12465v1) · [依据2](https://github.com/Zhu-Huixiang/embodied-world/blob/main/leaderboard/selection-2026-10-10.md)

原始引用记录与编辑证据分分别保留，计算细则见评分说明。

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
