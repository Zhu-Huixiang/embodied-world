# 共享网络的反向采样 · DDPM

从标准高斯逐步求μθ并加σz。

每步新z不同于训练ε；t1取z0；1000次共享参数调用，不是1000套网络。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md#35-把算法摊开训练一题生成一整套)

继续拆：[采样硬件与批量账单](runtime.md) · [xhat0不是下一步状态](estimate.md) · [共享中间状态再随机分叉](fork.md)。

[本篇星系](../ddpm.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md) · [原文依据](https://arxiv.org/pdf/2006.11239v2)
