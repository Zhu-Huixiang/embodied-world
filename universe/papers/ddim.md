# DDIM 星系

Denoising Diffusion Implicit Models

**导读** · Diffusion / Transformer 基础

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/ddim.md) · [原文](https://iclr.cc/virtual/2021/poster/2804) · [评分卡](../../leaderboard/papers/ddim/README.md)

构造共享相同加噪边缘分布的非马尔可夫过程，使训练仍然使用 DDPM 的噪声预测目标。推理则选择子时间序列和相应更新规则，确定性情形可以少步从噪声映射到数据。原文比较不同步数的生成速度、质量、插值和重建，揭示采样器改动无需等同于重新训练模型。

## 技术挂点

- [扩散去噪](../concepts/diffusion.md)：训练网络从带噪对象估计噪声或干净目标，生成时从噪声开始迭代恢复样本。

- [条件生成](../concepts/generation.md)：从一个条件生成多个可能输出，学习图像、视频或动作的分布而非只给一个均值。

## 本篇行星与卫星

- [扩散去噪](ddim/diffusion.md) · 初读挂点
- [条件生成](ddim/generation.md) · 初读挂点
- [本篇方法链路](ddim/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
