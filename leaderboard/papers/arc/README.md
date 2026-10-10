# ARC: A Reasoning Recipe for Robot Foundation Models

**ARC** · arXiv 2026 · 本版排名 112 · 综合分 **44.2 / 100**

[解读导读](../../../library/arc.md) · [视觉语言动作模型 VLA](../../../paper-map/README.md#track-vla) · [arXiv集锦](../../../arxiv/README.md#paper-arc)

[原文](https://arxiv.org/abs/2610.12386v1) · [PDF](https://arxiv.org/pdf/2610.12386v1) · [阅读卡片](../../../library/arc.md)

## 机制简析

给现有示范自动添“下一动作为什么合适、会造成什么”的推理轨迹，再按 VLA/WAM 架构适配推理与动作输出。

带着这个问题读：推理文字怎样成为动作条件，而不是另一段好看的解说？

初读判断：推理与控制的明确接口；初读关注自动标注质量、不同基础策略的匹配训练和零样本条件。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 0 | 30% |
| 创新性 | 87 | 20% |
| 实验与证据 | 76 | 20% |
| 学术影响 | 0 | 10% |
| 近期关注 | 0 | 5% |
| 复用价值 | 65 | 8% |
| 阅读价值 | 91 | 7% |

发表与刊会：预印本公开，正式发表贡献记0；创新与实验单独计分。


编辑深度：选题初读；评分记录：2026-10-10。

影响与关注采用独立证据评分：

- **学术影响 0**：本次2026-10-10补查范围内，独立采用证据仍在积累；按证据量表起点计0分。原文方法与作者实验分别进入创新、证据轴。 [依据1](https://arxiv.org/abs/2610.12386v1) · [依据2](https://github.com/Zhu-Huixiang/embodied-world/blob/main/leaderboard/selection-2026-10-10.md)
- **近期关注 0**：本次2026-10-10补查范围内，2025–2026的独立采用证据仍在积累；按证据量表起点计0分。原文方法与作者实验分别进入创新、证据轴。 [依据1](https://arxiv.org/abs/2610.12386v1) · [依据2](https://github.com/Zhu-Huixiang/embodied-world/blob/main/leaderboard/selection-2026-10-10.md)

原始引用记录与编辑证据分分别保留，计算细则见评分说明。

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
