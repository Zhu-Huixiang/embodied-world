# 从预测噪声到反向均值 · DDPM

网络εθ经解析系数换算为μθ。

均方误差最优输出是噪声条件均值，不从纯噪声找某张照片的前世；张量仍H×W×3。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md#32-反向均值把难猜的对象换一种写法)

继续拆：[噪声条件均值与score](score.md)。

[本篇星系](../ddpm.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md) · [原文依据](https://arxiv.org/pdf/2006.11239v2)
