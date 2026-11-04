# 一步物理连同梯度的计时 · ∇Mimic

同GPU同world数测完整step+tape+adjoint。

4096world/RTX PRO6000：1.78ms对MuJoCo Warp开放adjoint PR的20.5ms；11.5倍是完整带梯度步骤，非单独backward速度。

继续拆：[同算法更换仿真器](nm-isolation.md)。

[本篇星系](../nablamimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/nablamimic.md) · [原文依据](https://arxiv.org/pdf/2610.41654v1)
