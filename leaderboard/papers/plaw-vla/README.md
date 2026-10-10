# PLaW-VLA: Predictive Latent World Modeling for Vision-Language-Action Policies

**PLaW-VLA** · arXiv 2026 · 本版排名 115 · 综合分 **43.1 / 100**

[解读导读](../../../library/plaw-vla.md) · [视频动作模型与视觉推理](../../../paper-map/README.md#track-video-action) · [arXiv集锦](../../../arxiv/README.md#paper-plaw-vla)

[原文](https://arxiv.org/abs/2610.12285v1) · [PDF](https://arxiv.org/pdf/2610.12285v1) · [阅读卡片](../../../library/plaw-vla.md)

## 机制简析

预测面向任务的未来潜表示，再用结构化因果注意力让动作生成读取历史、任务和未来状态，减少无关像素重建。

带着这个问题读：怎样证明预测的未来表征真的帮助长程动作？

初读判断：有响应式策略与重建表示对照线索；初读优先看长程任务、未来预测和注意力结构消融。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 0 | 30% |
| 创新性 | 84 | 20% |
| 实验与证据 | 75 | 20% |
| 学术影响 | 0 | 10% |
| 近期关注 | 0 | 5% |
| 复用价值 | 63 | 8% |
| 阅读价值 | 89 | 7% |

发表与刊会：预印本公开，正式发表贡献记0；创新与实验单独计分。


编辑深度：选题初读；评分记录：2026-10-10。

影响与关注采用独立证据评分：

- **学术影响 0**：本次2026-10-10补查范围内，独立采用证据仍在积累；按证据量表起点计0分。原文方法与作者实验分别进入创新、证据轴。 [依据1](https://arxiv.org/abs/2610.12285v1) · [依据2](https://github.com/Zhu-Huixiang/embodied-world/blob/main/leaderboard/selection-2026-10-10.md)
- **近期关注 0**：本次2026-10-10补查范围内，2025–2026的独立采用证据仍在积累；按证据量表起点计0分。原文方法与作者实验分别进入创新、证据轴。 [依据1](https://arxiv.org/abs/2610.12285v1) · [依据2](https://github.com/Zhu-Huixiang/embodied-world/blob/main/leaderboard/selection-2026-10-10.md)

原始引用记录与编辑证据分分别保留，计算细则见评分说明。

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
