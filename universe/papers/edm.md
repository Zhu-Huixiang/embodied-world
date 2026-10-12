# EDM 星系

Elucidating the Design Space of Diffusion-Based Generative Models

**导读** · Diffusion / Transformer 基础

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/edm.md) · [原文](https://proceedings.neurips.cc/paper_files/paper/2022/hash/a98846e9d9cc01cfb87eb694d946ce6b-Abstract-Conference.html) · [评分卡](../../leaderboard/papers/edm/README.md)

把扩散过程的噪声参数化、采样求解器和网络预处理分别定义，减少不同实现之间的隐性差异。网络输入、输出和训练损失按噪声尺度预调节，推理使用更合适的时间离散与高阶求解。原文同时重用旧模型更换采样器、重训网络，比较质量与网络调用次数。

## 技术挂点

- [扩散去噪](../concepts/diffusion.md)：训练网络从带噪对象估计噪声或干净目标，生成时从噪声开始迭代恢复样本。

- [去噪网络预条件化](../concepts/preconditioning.md)：按噪声强度缩放网络输入、输出和跳接，使不同噪声级的训练更稳定。

- [条件生成](../concepts/generation.md)：从一个条件生成多个可能输出，学习图像、视频或动作的分布而非只给一个均值。

## 本篇行星与卫星

- [扩散去噪](edm/diffusion.md) · 初读挂点
- [去噪网络预条件化](edm/preconditioning.md) · 初读挂点
- [条件生成](edm/generation.md) · 初读挂点
- [本篇方法链路](edm/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
