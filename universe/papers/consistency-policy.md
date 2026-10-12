# Consistency Policy 星系

Consistency Policy: Accelerated Visuomotor Policies via Consistency Distillation

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/consistency-policy.md) · [原文](https://www.roboticsproceedings.org/rss20/p071.html) · [评分卡](../../leaderboard/papers/consistency-policy/README.md)

将多步扩散动作策略蒸馏为较少步的一致性策略，以减少推理步骤保留动作分布。

## 技术挂点

- [一致性生成](../concepts/consistency.md)：让同一生成轨迹上的不同噪声状态映射到相同干净目标，用于一步或少步生成。

- [扩散去噪](../concepts/diffusion.md)：训练网络从带噪对象估计噪声或干净目标，生成时从噪声开始迭代恢复样本。

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。

## 本篇行星与卫星

- [一致性生成](consistency-policy/consistency.md) · 初读挂点
- [扩散去噪](consistency-policy/diffusion.md) · 初读挂点
- [动作块](consistency-policy/chunk.md) · 初读挂点
- [本篇方法链路](consistency-policy/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
