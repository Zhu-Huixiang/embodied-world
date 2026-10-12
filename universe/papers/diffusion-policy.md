# Diffusion Policy 星系

Diffusion Policy: Visuomotor Policy Learning via Action Diffusion

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/diffusion-policy.md) · [原文](https://www.roboticsproceedings.org/rss19/p026.html) · [评分卡](../../leaderboard/papers/diffusion-policy/README.md)

对多步动作条件去噪，用视觉观测约束动作分布，滚动执行一段后再次观测与重规划。

## 技术挂点

- [扩散去噪](../concepts/diffusion.md)：训练网络从带噪对象估计噪声或干净目标，生成时从噪声开始迭代恢复样本。

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。

- [闭环滚动与历史偏移](../concepts/rollout.md)：重复预测、执行或生成，把新观测或模型历史接回后续计算。

## 本篇行星与卫星

- [扩散去噪](diffusion-policy/diffusion.md) · 初读挂点
- [动作块](diffusion-policy/chunk.md) · 初读挂点
- [闭环滚动与历史偏移](diffusion-policy/rollout.md) · 初读挂点
- [本篇方法链路](diffusion-policy/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
