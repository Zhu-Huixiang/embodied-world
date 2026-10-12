# DreamWaQ 星系

DreamWaQ: Learning Robust Quadrupedal Locomotion With Implicit Terrain Imagination via Deep Reinforcement Learning

**导读** · Locomotion 与运动适应

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamwaq.md) · [原文](https://ieeexplore.ieee.org/abstract/document/10161144/) · [评分卡](../../leaderboard/papers/dreamwaq/README.md)

从本体历史估计速度和隐环境表示，将其送给策略；训练时以重建/特权监督组织环境编码。

## 技术挂点

- [特权训练信息](../concepts/privileged.md)：训练用额外环境真值或教师信息，部署另用可获取输入估计或模仿。

- [变分自编码器 VAE](../concepts/vae.md)：编码器描述潜变量分布，解码器从潜变量重建样本，用重建与分布正则共同训练。

- [环境适应](../concepts/adaptation.md)：根据历史观测或环境信息调整策略，使动力学或地形变化仍可处理。

## 本篇行星与卫星

- [特权训练信息](dreamwaq/privileged.md) · 初读挂点
- [变分自编码器 VAE](dreamwaq/vae.md) · 初读挂点
- [环境适应](dreamwaq/adaptation.md) · 初读挂点
- [本篇方法链路](dreamwaq/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
