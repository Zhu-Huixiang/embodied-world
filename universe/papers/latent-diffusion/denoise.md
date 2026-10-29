# 同形状噪声监督 · Latent Diffusion

对自己加入的噪声做MSE。

随机抽t，UNet预测同形状epsilon；E/D冻结。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/latent-diffusion-2112.10752/README.md#预测噪声标签是自己刚加进去的答案)

继续拆：[U-Net时间条件](time.md)。

[本篇星系](../latent-diffusion.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/latent-diffusion-2112.10752/README.md) · [原文依据](https://arxiv.org/pdf/2112.10752v2)
