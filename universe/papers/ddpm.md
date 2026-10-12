# DDPM 星系

Denoising Diffusion Probabilistic Models

**导读** · Diffusion / Transformer 基础

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/ddpm.md) · [原文](https://proceedings.neurips.cc/paper/2020/hash/4c5bcfec8584af0d967f1ab10179ca4b-Abstract.html) · [评分卡](../../leaderboard/papers/ddpm/README.md)

正向过程逐步给数据加高斯噪声，训练时随机抽噪声时刻，让网络预测混入的噪声。反向生成从纯噪声开始，多步使用网络估计均值并采样，得到图像或换成动作序列后的条件样本。原文给出变分目标与简化去噪目标的联系，在 CIFAR-10 和 LSUN 评估图像生成质量。

## 技术挂点

- [扩散去噪](../concepts/diffusion.md)：训练网络从带噪对象估计噪声或干净目标，生成时从噪声开始迭代恢复样本。

- [条件生成](../concepts/generation.md)：从一个条件生成多个可能输出，学习图像、视频或动作的分布而非只给一个均值。

## 本篇行星与卫星

- [扩散去噪](ddpm/diffusion.md) · 初读挂点
- [条件生成](ddpm/generation.md) · 初读挂点
- [本篇方法链路](ddpm/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
