# 像素与结构损失 · 3DGS

0.8倍L1与0.2倍D-SSIM共同优化照片匹配。

L1看逐像素差，结构项看局部结构；梯度返回位置、形状、颜色和透明度。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/gaussian-splatting-2308.04079/README.md#51-d-区先让渲染结果接近真照片)

继续拆：[自适应密度控制](densify.md)。

[本篇星系](../gaussian-splatting.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/gaussian-splatting-2308.04079/README.md) · [原文依据](https://arxiv.org/abs/2308.04079v1)
