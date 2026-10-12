# TD-MPC2 星系

TD-MPC2: Scalable, Robust World Models for Continuous Control

**导读** · 世界模型与模型强化学习

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/td-mpc2.md) · [原文](https://proceedings.iclr.cc/paper_files/paper/2024/hash/cf73d57b6dcda32b293df7c2d5341f49-Abstract-Conference.html) · [评分卡](../../leaderboard/papers/td-mpc2/README.md)

共享潜世界模型、价值和规划结构跨多任务学习，处理不同奖励尺度与动作空间。

## 技术挂点

- [动作条件动力学](../concepts/dynamics.md)：以当前状态和动作预测下一状态或分布，建立“做这个动作会发生什么”的计算接口。

- [模型预测控制 MPC](../concepts/mpc.md)：在模型里比较未来动作序列，执行开头一段，用新观测重算下一轮。

- [价值估计与校准](../concepts/value.md)：估计未来累积收益，再用保守、分位或参考价值等约束减少误导。

## 本篇行星与卫星

- [动作条件动力学](td-mpc2/dynamics.md) · 初读挂点
- [模型预测控制 MPC](td-mpc2/mpc.md) · 初读挂点
- [价值估计与校准](td-mpc2/value.md) · 初读挂点
- [本篇方法链路](td-mpc2/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
