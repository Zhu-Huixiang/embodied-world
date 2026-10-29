# 噪声条件均值与score · DDPM

score是噪声分布log密度对输入的梯度。

−E[ε|xt]/sqrt(1−αbar)给出score；负号和尺度都要保留。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md#32-反向均值把难猜的对象换一种写法)

[本篇星系](../ddpm.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md) · [原文依据](https://arxiv.org/pdf/2006.11239v2)
