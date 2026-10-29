# 离散像素的高斯积分 · DDPM

8位整数像素概率由高斯在对应区间积分。

缩放到−1…1，间距2/255、半宽1/255，边界延伸无穷；不是直接用点密度当概率。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md#33-最后一脚连续数值怎么落回像素)

[本篇星系](../ddpm.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md) · [原文依据](https://arxiv.org/pdf/2006.11239v2)
