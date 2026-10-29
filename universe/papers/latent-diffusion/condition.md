# 交叉注意力条件接口 · Latent Diffusion

图像位置Q读取条件token的K/V。

匹配N×M，输出N×d；空间条件可通道拼接。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/latent-diffusion-2112.10752/README.md#33-条件机制文字如何进入图像的计算)

继续拆：[无分类器引导](cfg.md)。

[本篇星系](../latent-diffusion.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/latent-diffusion-2112.10752/README.md) · [原文依据](https://arxiv.org/pdf/2112.10752v2)
