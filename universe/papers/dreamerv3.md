# DreamerV3 星系

Mastering diverse control tasks through world models

**导读** · 世界模型与模型强化学习

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamerv3.md) · [原文](https://www.nature.com/articles/s41586-025-08744-2) · [评分卡](../../leaderboard/papers/dreamerv3/README.md)

以统一的世界模型、奖励价值尺度处理和优化设计覆盖多类控制任务，减少逐任务调参。

## 技术挂点

- [动作条件动力学](../concepts/dynamics.md)：以当前状态和动作预测下一状态或分布，建立“做这个动作会发生什么”的计算接口。

- [想象轨迹训练](../concepts/imagination.md)：在学到的动力学里滚动状态，用预测奖励和值训练策略，从而增加决策训练数据。

- [策略与价值学习](../concepts/actor-critic.md)：actor 产生动作，critic 估计长期收益；价值估计为策略改进提供方向。

## 本篇行星与卫星

- [动作条件动力学](dreamerv3/dynamics.md) · 初读挂点
- [想象轨迹训练](dreamerv3/imagination.md) · 初读挂点
- [策略与价值学习](dreamerv3/actor-critic.md) · 初读挂点
- [本篇方法链路](dreamerv3/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
