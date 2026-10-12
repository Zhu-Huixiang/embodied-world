# Extreme Parkour 星系

Extreme Parkour with Legged Robots

**导读** · Locomotion 与运动适应

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/extreme-parkour.md) · [原文](https://ieeexplore.ieee.org/document/10610200) · [评分卡](../../leaderboard/papers/extreme-parkour/README.md)

先在模拟中用特权地形训练策略，再把运动控制和行进方向一起蒸馏到深度图像学生。统一奖励让不同障碍上的动作自行形成，深度网络给策略提供地形潜变量与目标方向，本体策略输出关节命令。实机验证跨沟、上箱、斜坡等任务，并消融方向蒸馏与净空奖励。

## 技术挂点

- [特权训练信息](../concepts/privileged.md)：训练用额外环境真值或教师信息，部署另用可获取输入估计或模仿。

- [教师学生蒸馏](../concepts/distill.md)：用教师的预测或动作监督学生，让部署模型复制可用行为。

- [仿真到实机](../concepts/sim2real.md)：处理仿真动力学、感知和真实系统间的差异，通过随机化、辨识、残差或适配来迁移。

## 本篇行星与卫星

- [特权训练信息](extreme-parkour/privileged.md) · 初读挂点
- [教师学生蒸馏](extreme-parkour/distill.md) · 初读挂点
- [仿真到实机](extreme-parkour/sim2real.md) · 初读挂点
- [本篇方法链路](extreme-parkour/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
