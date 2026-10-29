# 固定β日程 · DDPM

T1000，β线性从1e−4到.02。

α=1−β，αbar连乘；终点信号系数约.00635。C只更新θ，不学习出题日程。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md#31-固定前向过程先别让出题人一起乱跑)

继续拆：[缩信号与控方差](variance.md)。

[本篇星系](../ddpm.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md) · [原文依据](https://arxiv.org/pdf/2006.11239v2)
