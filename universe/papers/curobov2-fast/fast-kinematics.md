# 共享连杆wrench与Jacobian列 · cuRoboV2-Fast

先计算连杆位姿，反向时复用每连杆汇总梯度。

每执行器收集后代连杆wrench并投影到运动方向，减少重复祖先遍历；IK需要显式Jacobian，轨迹优化直接用loss梯度。

继续拆：[模块时延不等于完整规划](fast-kernel-benchmark.md)。

[本篇星系](../curobov2-fast.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/curobov2-fast.md) · [原文依据](https://arxiv.org/pdf/2611.06913v1)
