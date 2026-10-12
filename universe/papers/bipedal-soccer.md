# Bipedal Soccer 星系

Learning agile soccer skills for a bipedal robot with deep reinforcement learning

**导读** · Locomotion 与运动适应

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/bipedal-soccer.md) · [原文](https://www.science.org/doi/10.1126/scirobotics.adi8022) · [评分卡](../../leaderboard/papers/bipedal-soccer/README.md)

先学习起身和足球等技能，再训练能在比赛状态下组合动作的策略；底层动作为二十维关节位置目标。MPO 更新策略和值函数，系统辨识、针对性的动力学随机化和扰动帮助模拟策略迁移到真实机器人。论文用一对一足球与脚本控制器对比行走、转向、起身和踢球表现。

## 技术挂点

- [策略与价值学习](../concepts/actor-critic.md)：actor 产生动作，critic 估计长期收益；价值估计为策略改进提供方向。

- [分层技能与计划](../concepts/skills.md)：高层选择目标或技能，低层负责具体执行，层次之间有明确接口。

- [仿真到实机](../concepts/sim2real.md)：处理仿真动力学、感知和真实系统间的差异，通过随机化、辨识、残差或适配来迁移。

## 本篇行星与卫星

- [策略与价值学习](bipedal-soccer/actor-critic.md) · 初读挂点
- [分层技能与计划](bipedal-soccer/skills.md) · 初读挂点
- [仿真到实机](bipedal-soccer/sim2real.md) · 初读挂点
- [本篇方法链路](bipedal-soccer/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
