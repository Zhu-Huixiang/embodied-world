# Dynamics Review 星系

A review of learning-based dynamics models for robotic manipulation

**导读** · 世界模型与模型强化学习

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/learned-dynamics-review.md) · [原文](https://www.science.org/doi/10.1126/scirobotics.adt1497) · [评分卡](../../leaderboard/papers/learned-dynamics-review/README.md)

以 POMDP/控制目标为入口，按像素、latent、粒子、关键点、物体中心表示比较动力学；再讨论感知和控制接口。

## 技术挂点

- [动作条件动力学](../concepts/dynamics.md)：以当前状态和动作预测下一状态或分布，建立“做这个动作会发生什么”的计算接口。

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。

## 本篇行星与卫星

- [动作条件动力学](learned-dynamics-review/dynamics.md) · 初读挂点
- [空间表示](learned-dynamics-review/spatial.md) · 初读挂点
- [表征空间](learned-dynamics-review/representation.md) · 初读挂点
- [本篇方法链路](learned-dynamics-review/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
