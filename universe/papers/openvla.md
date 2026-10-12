# OpenVLA 星系

OpenVLA: An Open-Source Vision-Language-Action Model

**导读** · 视觉语言动作模型 VLA

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/openvla.md) · [原文](https://proceedings.mlr.press/v270/kim25c.html) · [评分卡](../../leaderboard/papers/openvla/README.md)

把预训练视觉语言骨干适配到机器人示范，输出离散动作编号，并提供高效微调路线。

## 技术挂点

- [离散编码与量化](../concepts/quantization.md)：把连续向量或信号映射到有限码。动作、视频潜变量与世界模型状态都可能采用这种表示，码本和训练目标各不相同。

- [跨本体数据](../concepts/cross-body.md)：从多个机器人或人类收集经验，通过动作/观测适配接到共享学习系统。

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。

## 本篇行星与卫星

- [离散编码与量化](openvla/quantization.md) · 初读挂点
- [跨本体数据](openvla/cross-body.md) · 初读挂点
- [表征空间](openvla/representation.md) · 初读挂点
- [本篇方法链路](openvla/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
