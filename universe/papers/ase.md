# ASE 星系

ASE: Large-Scale Reusable Adversarial Skill Embeddings for Physically Simulated Characters

**导读** · 动作先验与全身技能

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/ase.md) · [原文](https://xbpeng.github.io/projects/ASE/) · [评分卡](../../leaderboard/papers/ase/README.md)

将潜技能条件与对抗动作先验联合训练，再让高层策略选择可复用的技能嵌入。

## 技术挂点

- [对抗动作模仿](../concepts/adversarial.md)：判别器区分参考与策略运动，将判别信号转成鼓励符合参考风格的奖励。

- [分层技能与计划](../concepts/skills.md)：高层选择目标或技能，低层负责具体执行，层次之间有明确接口。

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。

## 本篇行星与卫星

- [对抗动作模仿](ase/adversarial.md) · 初读挂点
- [分层技能与计划](ase/skills.md) · 初读挂点
- [表征空间](ase/representation.md) · 初读挂点
- [本篇方法链路](ase/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
