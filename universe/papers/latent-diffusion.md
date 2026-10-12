# Latent Diffusion 星系

High-Resolution Image Synthesis with Latent Diffusion Models

**导读** · Diffusion / Transformer 基础

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/latent-diffusion.md) · [原文](https://openaccess.thecvf.com/content/CVPR2022/html/Rombach_High-Resolution_Image_Synthesis_With_Latent_Diffusion_Models_CVPR_2022_paper.html) · [评分卡](../../leaderboard/papers/latent-diffusion/README.md)

先训练自动编码器，把高分辨率图像压成空间 latent；再在 latent 上训练扩散网络，最后解码为图像。文本或布局由条件编码器产生 token，并通过交叉注意力进入去噪网络。原文比较压缩程度、图像质量和计算成本，并评估文生图、修复与超分辨率。

## 技术挂点

- [扩散去噪](../concepts/diffusion.md)：训练网络从带噪对象估计噪声或干净目标，生成时从噪声开始迭代恢复样本。

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。

## 本篇行星与卫星

- [扩散去噪](latent-diffusion/diffusion.md) · 初读挂点
- [注意力](latent-diffusion/attention.md) · 初读挂点
- [表征空间](latent-diffusion/representation.md) · 初读挂点
- [本篇方法链路](latent-diffusion/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
