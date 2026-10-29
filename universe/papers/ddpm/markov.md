# 前向与反向马尔可夫链 · DDPM

每次转移只依赖当前状态。

q按固定规则从0到T；pθ从T到0，要学反向高斯均值。图中左右位置不决定时间方向。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md#21-两条链先别把箭头看反)

继续拆：[图像、噪声与批形状](shapes.md) · [固定β日程](schedule.md) · [直达任意噪声等级](marginal.md) · [已知x0的高斯后验](posterior.md)。

[本篇星系](../ddpm.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md) · [原文依据](https://arxiv.org/pdf/2006.11239v2)
