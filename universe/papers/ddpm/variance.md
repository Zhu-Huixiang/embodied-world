# 缩信号与控方差 · DDPM

每步先乘sqrt(1−β)再加sqrt(β)ε。

输入坐标方差若为1且噪声独立，输出方差仍1；是尺度计算，不假定图像分布本身是标准高斯。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md#22-加噪公式里为什么还要把原图缩小)

[本篇星系](../ddpm.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md) · [原文依据](https://arxiv.org/pdf/2006.11239v2)
