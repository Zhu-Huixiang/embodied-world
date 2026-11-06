# 用物体动力学构造教师力 · Ctrl-F

解析教师先计算六维目标力矩，再分配给接触通道。

位姿/速度误差经PD反馈和Newton–Euler动力学得到W*；悬空物体补偿重力，地面物体补偿Coulomb摩擦。教师使用训练时真实质量与特权状态。

继续拆：[抓取矩阵连接接触力和物体力矩](cf-allocation.md)。

[本篇星系](../ctrl-f.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/ctrl-f.md) · [原文依据](https://arxiv.org/pdf/2611.05507v1)
