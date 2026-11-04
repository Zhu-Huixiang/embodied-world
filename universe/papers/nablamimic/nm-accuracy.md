# 有限差分校验导数 · ∇Mimic

用高精度MuJoCo作参考验证实现，而非用学习成功代替数值正确。

16384 held-out状态，梯度每组至多256；float64中心差分步长1e-6。Table7位置/速度/动作VJP相对误差中位数3.6e-5/1.0e-5/1.9e-6，G5/G6是G0子集。

[本篇星系](../nablamimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/nablamimic.md) · [原文依据](https://arxiv.org/pdf/2610.41654v1)
