# 已知x0的高斯后验 · DDPM

训练已知x0时q(xt−1|xt,x0)可算。

后验均值是x0与xt的加权和、系数标量；生成时x0不可见，用μθ给出反向分布。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md#23-训练知道原图生成不知道正好差在这里)

[本篇星系](../ddpm.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md) · [原文依据](https://arxiv.org/pdf/2006.11239v2)
