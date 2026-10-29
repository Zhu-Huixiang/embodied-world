# Latent Diffusion 星系

High-Resolution Image Synthesis with Latent Diffusion Models

**已精讲** · Diffusion / Transformer 基础

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/latent-diffusion-2112.10752/README.md) · [原文](https://openaccess.thecvf.com/content/CVPR2022/html/Rombach_High-Resolution_Image_Synthesis_With_Latent_Diffusion_Models_CVPR_2022_paper.html) · [评分卡](../../leaderboard/papers/latent-diffusion/README.md)

先训练自动编码器，把高分辨率图像压成空间 latent；再在 latent 上训练扩散网络，最后解码为图像。文本或布局由条件编码器产生 token，并通过交叉注意力进入去噪网络。原文比较压缩程度、图像质量和计算成本，并评估文生图、修复与超分辨率。

## 技术挂点

- [扩散去噪](../concepts/diffusion.md)：训练网络从带噪对象估计噪声或干净目标，生成时从噪声开始迭代恢复样本。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/latent-diffusion-2112.10752/README.md#32-潜空间扩散随机抽一道题学会整条去噪链)

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/latent-diffusion-2112.10752/README.md#33-条件机制文字如何进入图像的计算)

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/latent-diffusion-2112.10752/README.md#31-感知压缩先把画面装进一个靠谱的小空间)

- [条件生成](../concepts/generation.md)：从一个条件生成多个可能输出，学习图像、视频或动作的分布而非只给一个均值。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/latent-diffusion-2112.10752/README.md#6-结论回收三个问题再接上具身智能)

## 本篇行星与卫星

- [扩散去噪](latent-diffusion/diffusion.md) · 已讲解
- [注意力](latent-diffusion/attention.md) · 已讲解
- [表征空间](latent-diffusion/representation.md) · 已讲解
- [条件生成](latent-diffusion/generation.md) · 已讲解
- [本篇方法链路](latent-diffusion/method-chain.md) · 初读挂点
- [感知压缩的计算分工](latent-diffusion/compression.md) · 已讲解
- [重建、感知、对抗与正则](latent-diffusion/loss.md) · 已讲解
- [潜变量前向加噪](latent-diffusion/noise.md) · 已讲解
- [同形状噪声监督](latent-diffusion/denoise.md) · 已讲解
- [U-Net时间条件](latent-diffusion/time.md) · 已讲解
- [潜空间采样再解码](latent-diffusion/sample.md) · 已讲解
- [交叉注意力条件接口](latent-diffusion/condition.md) · 已讲解
- [无分类器引导](latent-diffusion/cfg.md) · 已讲解
- [压缩倍率与质量速度](latent-diffusion/compression-choice.md) · 已讲解
- [像素相似与视觉真实](latent-diffusion/metrics.md) · 已讲解
- [补图与多答案](latent-diffusion/inpaint.md) · 已讲解
- [任务相关细节的表示检验](latent-diffusion/robotics.md) · 已讲解

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
