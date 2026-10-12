# Dreamer 星系

Dream to Control: Learning Behaviors by Latent Imagination

**导读** · 世界模型与模型强化学习

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamer.md) · [原文](https://research.google/pubs/dream-to-control-learning-behaviors-by-latent-imagination/) · [评分卡](../../leaderboard/papers/dreamer/README.md)

学习潜动力学世界模型，在想象轨迹里以价值反馈优化actor，把像素预测转成决策训练信号。

## 技术挂点

- [动作条件动力学](../concepts/dynamics.md)：以当前状态和动作预测下一状态或分布，建立“做这个动作会发生什么”的计算接口。

- [想象轨迹训练](../concepts/imagination.md)：在学到的动力学里滚动状态，用预测奖励和值训练策略，从而增加决策训练数据。

- [策略与价值学习](../concepts/actor-critic.md)：actor 产生动作，critic 估计长期收益；价值估计为策略改进提供方向。

## 本篇行星与卫星

- [动作条件动力学](dreamer/dynamics.md) · 初读挂点
- [想象轨迹训练](dreamer/imagination.md) · 初读挂点
- [策略与价值学习](dreamer/actor-critic.md) · 初读挂点
- [本篇方法链路](dreamer/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
