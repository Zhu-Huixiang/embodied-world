# ExBody 星系

Expressive Whole-Body Control for Humanoid Robots

**导读** · Locomotion 与运动适应

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/exbody.md) · [原文](https://www.roboticsproceedings.org/rss20/p107.html) · [评分卡](../../leaderboard/papers/exbody/README.md)

从人类动作库筛选并重定向姿态，训练时要求机器人上半身跟随关节和关键点目标。下半身放松逐关节模仿约束，改为跟随根速度和姿态命令，以留出平衡和行走空间。原文对照完整身体跟踪、分开策略与初始化方式，实机展示行走和表达动作。

## 技术挂点

- [运动重定向](../concepts/retarget.md)：把人或另一种机器人的运动转换到目标本体的关节、末端与可达范围。

- [全身控制与执行](../concepts/wbc.md)：将运动目标、机器人状态和约束转成关节目标或力矩，协调腿、手臂与底盘。

- [动作先验](../concepts/motion-prior.md)：从运动数据学习自然动作规律，再把它接进物理控制或技能选择。

## 本篇行星与卫星

- [运动重定向](exbody/retarget.md) · 初读挂点
- [全身控制与执行](exbody/wbc.md) · 初读挂点
- [动作先验](exbody/motion-prior.md) · 初读挂点
- [本篇方法链路](exbody/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
