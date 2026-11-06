# 本篇方法链路 · cuRoboV2-Fast

用三次B样条降低轨迹优化变量耦合；直线种子不足时GPU双向RRT补路线。随后TimeOpt固定几何、以路径速度平方样条非均匀分配时间，局部支持产生带状Newton系统，预测校正复用Cholesky。运动学、碰撞与RNEA直接梯度共同减少每次迭代成本，负载惯量可运行时更新。

用三次B样条降低轨迹优化变量耦合；直线种子不足时GPU双向RRT补路线。随后TimeOpt固定几何、以路径速度平方样条非均匀分配时间，局部支持产生带状Newton系统，预测校正复用Cholesky。运动学、碰撞与RNEA直接梯度共同减少每次迭代成本，负载惯量可运行时更新。

[本篇星系](../curobov2-fast.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/curobov2-fast.md) · [原文依据](https://arxiv.org/abs/2611.06913v1)
