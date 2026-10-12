# AMP 星系

AMP: Adversarial Motion Priors for Stylized Physics-Based Character Control

**导读** · 动作先验与全身技能

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/amp.md) · [原文](https://xbpeng.github.io/projects/AMP/) · [评分卡](../../leaderboard/papers/amp/README.md)

判别器区分参考与策略动作转移，把模仿先验变成奖励，减少逐帧跟踪的限制。

## 技术挂点

- [对抗动作模仿](../concepts/adversarial.md)：判别器区分参考与策略运动，将判别信号转成鼓励符合参考风格的奖励。

- [动作先验](../concepts/motion-prior.md)：从运动数据学习自然动作规律，再把它接进物理控制或技能选择。

- [强化学习](../concepts/rl.md)：通过奖励和值评估改进策略，研究动作如何改变长期回报。

## 本篇行星与卫星

- [对抗动作模仿](amp/adversarial.md) · 初读挂点
- [动作先验](amp/motion-prior.md) · 初读挂点
- [强化学习](amp/rl.md) · 初读挂点
- [本篇方法链路](amp/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
