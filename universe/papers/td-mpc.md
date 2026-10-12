# TD-MPC 星系

Temporal Difference Learning for Model Predictive Control

**导读** · 世界模型与模型强化学习

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/td-mpc.md) · [原文](https://proceedings.mlr.press/v162/hansen22a.html) · [评分卡](../../leaderboard/papers/td-mpc/README.md)

学习用于奖励和值预测的潜动力学，结合短期模型预测控制与终端价值选择连续动作。

## 技术挂点

- [动作条件动力学](../concepts/dynamics.md)：以当前状态和动作预测下一状态或分布，建立“做这个动作会发生什么”的计算接口。

- [模型预测控制 MPC](../concepts/mpc.md)：在模型里比较未来动作序列，执行开头一段，用新观测重算下一轮。

- [价值估计与校准](../concepts/value.md)：估计未来累积收益，再用保守、分位或参考价值等约束减少误导。

## 本篇行星与卫星

- [动作条件动力学](td-mpc/dynamics.md) · 初读挂点
- [模型预测控制 MPC](td-mpc/mpc.md) · 初读挂点
- [价值估计与校准](td-mpc/value.md) · 初读挂点
- [本篇方法链路](td-mpc/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
