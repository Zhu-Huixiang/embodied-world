# Agile Flight 星系

Learning high-speed flight in the wild

**导读** · Locomotion 与运动适应

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/agile-flight.md) · [原文](https://www.science.org/doi/10.1126/scirobotics.abg5810) · [评分卡](../../leaderboard/papers/agile-flight/README.md)

利用仿真专家监督视觉导航策略，再转移到高速野外飞行，连接感知、轨迹规划与实际反应。

## 技术挂点

- [教师学生蒸馏](../concepts/distill.md)：用教师的预测或动作监督学生，让部署模型复制可用行为。

- [仿真到实机](../concepts/sim2real.md)：处理仿真动力学、感知和真实系统间的差异，通过随机化、辨识、残差或适配来迁移。

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。

## 本篇行星与卫星

- [教师学生蒸馏](agile-flight/distill.md) · 初读挂点
- [仿真到实机](agile-flight/sim2real.md) · 初读挂点
- [空间表示](agile-flight/spatial.md) · 初读挂点
- [本篇方法链路](agile-flight/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
