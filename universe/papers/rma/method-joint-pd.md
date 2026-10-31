# 目标角经PD变成关节力矩 · RMA

动作接口是关节位置控制：角度误差提供恢复力矩，角速度误差提供阻尼。

实机固定Kp=55、Kd=0.8，目标角速度为0。基础策略输出的是12个期望角，而非直接输出12个力矩。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md#41-环境与动作接口)

[本篇星系](../rma.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md) · [原文依据](https://www.roboticsproceedings.org/rss17/p011.pdf)
