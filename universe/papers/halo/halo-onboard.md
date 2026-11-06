# 两台机载计算机分开语义与实时控制 · HALO

Mac mini承担编排和运动生成，G1原装Jetson Orin NX执行感知跟踪。

M4 Pro 64GB与Orin通过ZeroMQ异步联动；生成器约3Hz、跟踪器50Hz。TableIX生成器单独152ms、共服155ms，编排器单独0.72s、共服1.46s；这些是模型推理延迟，不是每次控制周期。

[本篇星系](../halo.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/halo.md) · [原文依据](https://arxiv.org/pdf/2611.06908v1)
