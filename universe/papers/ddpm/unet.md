# U-Net特征尺度与跳连 · DDPM

下采样后上采样，并连接同分辨率早期特征。

CIFAR32/16/8/4空间尺度，最后回3通道；跳连与残差是不同层面的连接。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md#36-打开-b-区u-net-里面怎样处理图像和时间)

继续拆：[正弦时间嵌入](time.md) · [卷积残差块与GroupNorm](residual.md) · [16×16空间注意力](spatial-attention.md)。

[本篇星系](../ddpm.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md) · [原文依据](https://arxiv.org/pdf/2006.11239v2)
