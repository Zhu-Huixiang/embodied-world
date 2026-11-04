# 单机器人融合求导引擎 · ∇Mimic

把物理仿真与反向传播从大量通用kernel调度变为专用计算。

Unitree G1特化、31刚体、502接触对、平地/球/胶囊；每world一个warp，正向每子步2kernel，整控制步反向1megakernel。

继续拆：[接触解最优条件的隐式求导](nm-adjoint.md) · [一步物理连同梯度的计时](nm-speed.md) · [专用引擎与仿真适用范围](nm-limit.md)。

[本篇星系](../nablamimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/nablamimic.md) · [原文依据](https://arxiv.org/pdf/2610.41654v1)
