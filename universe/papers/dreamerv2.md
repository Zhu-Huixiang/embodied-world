# DreamerV2 星系

Mastering Atari with Discrete World Models

**导读** · 世界模型与模型强化学习

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamerv2.md) · [原文](https://research.google/pubs/mastering-atari-with-discrete-world-models/) · [评分卡](../../leaderboard/papers/dreamerv2/README.md)

将世界模型潜状态换成离散表示，利用想象轨迹训练策略，重点检查Atari学习表现。

## 技术挂点

- [动作条件动力学](../concepts/dynamics.md)：以当前状态和动作预测下一状态或分布，建立“做这个动作会发生什么”的计算接口。

- [想象轨迹训练](../concepts/imagination.md)：在学到的动力学里滚动状态，用预测奖励和值训练策略，从而增加决策训练数据。

- [离散编码与量化](../concepts/quantization.md)：把连续向量或信号映射到有限码。动作、视频潜变量与世界模型状态都可能采用这种表示，码本和训练目标各不相同。

## 本篇行星与卫星

- [动作条件动力学](dreamerv2/dynamics.md) · 初读挂点
- [想象轨迹训练](dreamerv2/imagination.md) · 初读挂点
- [离散编码与量化](dreamerv2/quantization.md) · 初读挂点
- [本篇方法链路](dreamerv2/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
