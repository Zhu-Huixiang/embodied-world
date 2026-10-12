# Consistency Models 星系

Consistency Models

**导读** · Diffusion / Transformer 基础

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/consistency-models.md) · [原文](https://proceedings.mlr.press/v202/song23a.html) · [评分卡](../../leaderboard/papers/consistency-models/README.md)

学习一个映射，使概率流 ODE 同一轨迹上的不同噪声点都输出同一个干净样本。蒸馏版由教师扩散模型和求解器产生相邻轨迹点，训练版则直接通过相邻噪声尺度的一致性约束学习。原文在标准图像数据集比较一步、少步生成和编辑，机器人策略将同类映射用于压缩动作采样延迟。

## 技术挂点

- [一致性生成](../concepts/consistency.md)：让同一生成轨迹上的不同噪声状态映射到相同干净目标，用于一步或少步生成。

- [条件生成](../concepts/generation.md)：从一个条件生成多个可能输出，学习图像、视频或动作的分布而非只给一个均值。

## 本篇行星与卫星

- [一致性生成](consistency-models/consistency.md) · 初读挂点
- [条件生成](consistency-models/generation.md) · 初读挂点
- [本篇方法链路](consistency-models/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
