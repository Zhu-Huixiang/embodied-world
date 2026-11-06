# RNEA物理逆动力学 · cuRoboV2-Fast

给定关节位置、速度和加速度，计算所需关节力矩。

此处逆动力学是刚体Newton–Euler递推，不是从相邻视频推断动作的学习模型；直接反传loss梯度避免完整导数矩阵。

继续拆：[运行时更新负载惯量](fast-payload.md)。

[本篇星系](../curobov2-fast.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/curobov2-fast.md) · [原文依据](https://arxiv.org/pdf/2611.06913v1)
