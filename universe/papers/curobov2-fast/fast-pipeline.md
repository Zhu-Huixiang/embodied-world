# 先直线、必要时RRT再精修 · cuRoboV2-Fast

先尝试直线初值，失败时以几何路线初始化优化。

IK、可选GPU RRT、B样条几何优化、TimeOpt与最终检查组成规划链；不是每次调用都运行RRT。

继续拆：[有界双向并行RRT](fast-rrt.md) · [三次B样条位置控制点](fast-position-spline.md) · [共享连杆wrench与Jacobian列](fast-kinematics.md) · [包围盒剪枝与半段距离复用](fast-collision.md) · [RNEA物理逆动力学](fast-rnea.md) · [抓取与转移分两次规划](fast-grasp.md)。

[本篇星系](../curobov2-fast.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/curobov2-fast.md) · [原文依据](https://arxiv.org/pdf/2611.06913v1)
