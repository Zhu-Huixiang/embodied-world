# RMA 星系

RMA: Rapid Motor Adaptation for Legged Robots

**导读** · Locomotion 与运动适应

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/rma.md) · [原文](https://www.roboticsproceedings.org/rss17/p011.html) · [评分卡](../../leaderboard/papers/rma/README.md)

训练利用特权环境信息的基础策略，部署用状态动作历史估计环境编码，在线适配腿足控制。

## 技术挂点

- [特权训练信息](../concepts/privileged.md)：训练用额外环境真值或教师信息，部署另用可获取输入估计或模仿。

- [环境适应](../concepts/adaptation.md)：根据历史观测或环境信息调整策略，使动力学或地形变化仍可处理。

- [仿真到实机](../concepts/sim2real.md)：处理仿真动力学、感知和真实系统间的差异，通过随机化、辨识、残差或适配来迁移。

## 本篇行星与卫星

- [特权训练信息](rma/privileged.md) · 初读挂点
- [环境适应](rma/adaptation.md) · 初读挂点
- [仿真到实机](rma/sim2real.md) · 初读挂点
- [本篇方法链路](rma/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
