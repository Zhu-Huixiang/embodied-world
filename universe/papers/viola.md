# VIOLA 星系

VioLA: Learning Generalist Humanoid Control Policies from Human Data

**导读** · 视觉语言动作模型 VLA

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/viola.md) · [原文](https://arxiv.org/abs/2610.12435v1) · [评分卡](../../leaderboard/papers/viola/README.md)

VLA 预测身体与手部运动 latent，预训练控制器负责执行；运动编码器把人类示范映射到同一空间，扩大可监督动作池。

## 技术挂点

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。

- [动作先验](../concepts/motion-prior.md)：从运动数据学习自然动作规律，再把它接进物理控制或技能选择。

- [跨本体数据](../concepts/cross-body.md)：从多个机器人或人类收集经验，通过动作/观测适配接到共享学习系统。

## 本篇行星与卫星

- [表征空间](viola/representation.md) · 初读挂点
- [动作先验](viola/motion-prior.md) · 初读挂点
- [跨本体数据](viola/cross-body.md) · 初读挂点
- [本篇方法链路](viola/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
