# 变分账本的三部分 · DDPM

负对数似然上界分成LT、各步KL、L0。

固定前向令LT与θ无关；中间转移比较高斯；末端对应离散像素概率。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md#31-固定前向过程先别让出题人一起乱跑)

继续拆：[高斯KL与时间权重](gaussian-kl.md) · [离散像素的高斯积分](decoder.md) · [逐步编码与码率失真](rate.md)。

[本篇星系](../ddpm.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md) · [原文依据](https://arxiv.org/pdf/2006.11239v2)
