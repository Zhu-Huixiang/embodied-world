# EfficientZero V2 星系

EfficientZero V2: Mastering Discrete and Continuous Control with Limited Data

**导读** · 世界模型与模型强化学习

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/efficientzero-v2.md) · [原文](https://proceedings.mlr.press/v235/wang24at.html) · [评分卡](../../leaderboard/papers/efficientzero-v2/README.md)

表示函数得到潜状态，动力学函数接收动作并预测潜状态与奖励，策略和值网络为搜索提供先验。连续动作下先采样候选动作，再用基于 Gumbel 的树搜索改善策略，并用搜索产生价值目标以利用旧经验。实验按有限交互预算比较离散和连续、图像和低维输入任务。

## 技术挂点

- [动作条件动力学](../concepts/dynamics.md)：以当前状态和动作预测下一状态或分布，建立“做这个动作会发生什么”的计算接口。

- [树搜索与轨迹搜索](../concepts/search.md)：展开候选动作或轨迹，用预测价值挑选可执行方案。

- [价值估计与校准](../concepts/value.md)：估计未来累积收益，再用保守、分位或参考价值等约束减少误导。

## 本篇行星与卫星

- [动作条件动力学](efficientzero-v2/dynamics.md) · 初读挂点
- [树搜索与轨迹搜索](efficientzero-v2/search.md) · 初读挂点
- [价值估计与校准](efficientzero-v2/value.md) · 初读挂点
- [本篇方法链路](efficientzero-v2/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
