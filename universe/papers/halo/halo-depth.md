# 机器人自己的遮挡也要进入深度 · HALO

从双目红外估计局部深度，把地面和物体接触信息送入跟踪器。

LiteAnyStereo处理真实IR；深度截在0.2–2.5m，log(1+d)并降到48×84。仿真包含身体自遮挡；不是用高层RGB语义特征代替近身几何。

[本篇星系](../halo.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/halo.md) · [原文依据](https://arxiv.org/pdf/2611.06908v1)
