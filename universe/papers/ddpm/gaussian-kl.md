# 高斯KL与时间权重 · DDPM

固定协方差下KL可化成加权噪声平方误差。

wt含β²/[2σ²α(1−αbar)]，随时间变化；去权重会改变训练重心。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md#34-简化损失删掉权重训练重点跟着变了)

[本篇星系](../ddpm.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md) · [原文依据](https://arxiv.org/pdf/2006.11239v2)
