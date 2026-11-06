# 三次B样条位置控制点 · cuRoboV2-Fast

K×d个自由控制点描述d关节的连续轨迹。

每个轨迹样本只依赖四个相邻控制点，一次求位置、速度、加速度与jerk；增加检查采样密度不增加优化变量数。

继续拆：[按控制点收集梯度](fast-gradient-gather.md) · [固定路径上的非均匀时间分配](fast-timeopt.md) · [同IK种子的收敛消融](fast-convergence.md)。

[本篇星系](../curobov2-fast.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/curobov2-fast.md) · [原文依据](https://arxiv.org/pdf/2611.06913v1)
