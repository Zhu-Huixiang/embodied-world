# 固定路径上的非均匀时间分配 · cuRoboV2-Fast

TimeOpt保持q(s)几何不变，只优化沿路径的速度。

另一个三次B样条表示路径速度平方x(s)，时间为对1/sqrt(x)积分；位置控制点与时间控制点不能混同。

继续拆：[速度加速度jerk与力矩约束](fast-sampled-constraints.md) · [固定路径力矩仿射化](fast-affine-torque.md) · [局部支持带来的带状Newton系统](fast-banded.md) · [TimeOpt额外收益](fast-timing-ablation.md)。

[本篇星系](../curobov2-fast.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/curobov2-fast.md) · [原文依据](https://arxiv.org/pdf/2611.06913v1)
