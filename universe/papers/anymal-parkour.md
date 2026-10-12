# ANYmal Parkour 星系

ANYmal parkour: Learning agile navigation for quadrupedal robots

**导读** · Locomotion 与运动适应

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/anymal-parkour.md) · [原文](https://www.science.org/doi/10.1126/scirobotics.adi7566) · [评分卡](../../leaderboard/papers/anymal-parkour/README.md)

先训练跳、爬、蹲和行走等低层策略，高层导航策略依据感知重建的环境选择技能和目标。感知模块从遮挡、噪声输入重建障碍，使高层决策了解各技能可完成的动作范围。原文在连续障碍的实机导航中验证模拟训练链路。

## 技术挂点

- [分层技能与计划](../concepts/skills.md)：高层选择目标或技能，低层负责具体执行，层次之间有明确接口。

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。

- [仿真到实机](../concepts/sim2real.md)：处理仿真动力学、感知和真实系统间的差异，通过随机化、辨识、残差或适配来迁移。

## 本篇行星与卫星

- [分层技能与计划](anymal-parkour/skills.md) · 初读挂点
- [空间表示](anymal-parkour/spatial.md) · 初读挂点
- [仿真到实机](anymal-parkour/sim2real.md) · 初读挂点
- [本篇方法链路](anymal-parkour/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
