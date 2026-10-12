# Flow Matching 星系

Flow Matching for Generative Modeling

**导读** · Diffusion / Transformer 基础

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/flow-matching.md) · [原文](https://iclr.cc/virtual/2023/poster/11309) · [评分卡](../../leaderboard/papers/flow-matching/README.md)

给噪声与数据之间指定一个条件概率路径，直接回归该路径的目标速度场，训练时不用数值模拟完整 ODE。条件流匹配的目标在梯度层面对应难直接计算的边缘流目标；生成时才用求解器沿学习的速度场从噪声走向数据。原文比较扩散型路径与最优传输型插值，在 ImageNet 检查样本质量、似然和速度。

## 技术挂点

- [Flow Matching](../concepts/flow.md)：给噪声到数据指定概率路径，回归沿路径的速度场；生成时数值积分这个场。

- [条件生成](../concepts/generation.md)：从一个条件生成多个可能输出，学习图像、视频或动作的分布而非只给一个均值。

## 本篇行星与卫星

- [Flow Matching](flow-matching/flow.md) · 初读挂点
- [条件生成](flow-matching/generation.md) · 初读挂点
- [本篇方法链路](flow-matching/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
