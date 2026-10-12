# Legged Gym 星系

Learning to Walk in Minutes Using Massively Parallel Deep Reinforcement Learning

**导读** · Locomotion 与运动适应

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/walk-in-minutes.md) · [原文](https://proceedings.mlr.press/v164/rudin22a.html) · [评分卡](../../leaderboard/papers/walk-in-minutes/README.md)

物理仿真和 PPO 训练都留在 GPU 上，用大量并行环境快速组成更新批次。地形课程根据机器人前进表现升降难度，任务课程逐步扩大命令范围。原文分析大并行下训练组件并把 ANYmal 策略转到实机，公开 legged_gym。

## 技术挂点

- [PPO 与并行模拟](../concepts/ppo.md)：用受约束的策略更新与大量模拟轨迹训练控制；并行度改变每轮数据和训练开销。

- [仿真到实机](../concepts/sim2real.md)：处理仿真动力学、感知和真实系统间的差异，通过随机化、辨识、残差或适配来迁移。

- [环境适应](../concepts/adaptation.md)：根据历史观测或环境信息调整策略，使动力学或地形变化仍可处理。

## 本篇行星与卫星

- [PPO 与并行模拟](walk-in-minutes/ppo.md) · 初读挂点
- [仿真到实机](walk-in-minutes/sim2real.md) · 初读挂点
- [环境适应](walk-in-minutes/adaptation.md) · 初读挂点
- [本篇方法链路](walk-in-minutes/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
