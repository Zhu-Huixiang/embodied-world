# Perceptive Locomotion 星系

Learning robust perceptive locomotion for quadrupedal robots in the wild

**导读** · Locomotion 与运动适应

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/perceptive-loco.md) · [原文](https://www.science.org/doi/10.1126/scirobotics.abk2822) · [评分卡](../../leaderboard/papers/perceptive-loco/README.md)

让地形感知与本体反馈共同支持腿足策略，在复杂户外地形中考察感知失效和控制鲁棒性。

## 技术挂点

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。

- [环境适应](../concepts/adaptation.md)：根据历史观测或环境信息调整策略，使动力学或地形变化仍可处理。

- [仿真到实机](../concepts/sim2real.md)：处理仿真动力学、感知和真实系统间的差异，通过随机化、辨识、残差或适配来迁移。

## 本篇行星与卫星

- [空间表示](perceptive-loco/spatial.md) · 初读挂点
- [环境适应](perceptive-loco/adaptation.md) · 初读挂点
- [仿真到实机](perceptive-loco/sim2real.md) · 初读挂点
- [本篇方法链路](perceptive-loco/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
