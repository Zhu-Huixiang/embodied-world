# DP3 星系

3D Diffusion Policy: Generalizable Visuomotor Policy Learning via Simple 3D Representations

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dp3.md) · [原文](https://www.roboticsproceedings.org/rss20/p067.html) · [评分卡](../../leaderboard/papers/dp3/README.md)

以简洁点云编码器提供三维条件，用扩散生成动作，观察几何表示对泛化的影响。

## 技术挂点

- [点云与三维体素](../concepts/point-cloud.md)：点云用三维点记录几何，网络从点的位置与特征构造空间表示。

- [扩散去噪](../concepts/diffusion.md)：训练网络从带噪对象估计噪声或干净目标，生成时从噪声开始迭代恢复样本。

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。

## 本篇行星与卫星

- [点云与三维体素](dp3/point-cloud.md) · 初读挂点
- [扩散去噪](dp3/diffusion.md) · 初读挂点
- [动作块](dp3/chunk.md) · 初读挂点
- [本篇方法链路](dp3/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
