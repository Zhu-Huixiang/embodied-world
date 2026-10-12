# MuZero 星系

Mastering Atari, Go, chess and shogi by planning with a learned model

**导读** · 世界模型与模型强化学习

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/muzero.md) · [原文](https://www.nature.com/articles/s41586-020-03051-4) · [评分卡](../../leaderboard/papers/muzero/README.md)

表示网络从观测历史得到潜状态，动力学网络在动作条件下预测下一潜状态和奖励，预测网络给出策略先验和值。MCTS 在这些潜状态里展开候选动作，搜索产生的策略和值再监督网络。Nature 论文比较棋类与 Atari；这里关注的是规划表征，而不是实机机器人结论。

## 技术挂点

- [动作条件动力学](../concepts/dynamics.md)：以当前状态和动作预测下一状态或分布，建立“做这个动作会发生什么”的计算接口。

- [树搜索与轨迹搜索](../concepts/search.md)：展开候选动作或轨迹，用预测价值挑选可执行方案。

- [价值估计与校准](../concepts/value.md)：估计未来累积收益，再用保守、分位或参考价值等约束减少误导。

## 本篇行星与卫星

- [动作条件动力学](muzero/dynamics.md) · 初读挂点
- [树搜索与轨迹搜索](muzero/search.md) · 初读挂点
- [价值估计与校准](muzero/value.md) · 初读挂点
- [本篇方法链路](muzero/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
