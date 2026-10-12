# ASAP 星系

ASAP: Aligning Simulation and Real-World Physics for Learning Agile Humanoid Whole-Body Skills

**导读** · Locomotion 与运动适应

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/asap.md) · [原文](https://www.roboticsproceedings.org/rss21/p066.html) · [评分卡](../../leaderboard/papers/asap/README.md)

先在模拟里训练人类动作跟踪策略，再在实机执行并记录轨迹。用真实轨迹训练 delta action 模型，找出能让模拟运动贴近真实运动的动作修正，把它接回模拟器后微调跟踪策略。原文比较跨模拟器和 Unitree G1 实机迁移，并对照系统辨识、域随机化与动力学残差。

## 技术挂点

- [运动重定向](../concepts/retarget.md)：把人或另一种机器人的运动转换到目标本体的关节、末端与可达范围。

- [动作条件动力学](../concepts/dynamics.md)：以当前状态和动作预测下一状态或分布，建立“做这个动作会发生什么”的计算接口。

- [仿真到实机](../concepts/sim2real.md)：处理仿真动力学、感知和真实系统间的差异，通过随机化、辨识、残差或适配来迁移。

## 本篇行星与卫星

- [运动重定向](asap/retarget.md) · 初读挂点
- [动作条件动力学](asap/dynamics.md) · 初读挂点
- [仿真到实机](asap/sim2real.md) · 初读挂点
- [本篇方法链路](asap/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
