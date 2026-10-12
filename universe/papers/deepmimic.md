# DeepMimic 星系

DeepMimic: Example-Guided Deep Reinforcement Learning of Physics-Based Character Skills

**导读** · 动作先验与全身技能

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/deepmimic.md) · [原文](https://xbpeng.github.io/projects/DeepMimic/) · [评分卡](../../leaderboard/papers/deepmimic/README.md)

任务奖励与参考动作跟踪奖励共同训练物理角色策略，使动作技能能在动态扰动后恢复。

## 技术挂点

- [动作先验](../concepts/motion-prior.md)：从运动数据学习自然动作规律，再把它接进物理控制或技能选择。

- [强化学习](../concepts/rl.md)：通过奖励和值评估改进策略，研究动作如何改变长期回报。

- [全身控制与执行](../concepts/wbc.md)：将运动目标、机器人状态和约束转成关节目标或力矩，协调腿、手臂与底盘。

## 本篇行星与卫星

- [动作先验](deepmimic/motion-prior.md) · 初读挂点
- [强化学习](deepmimic/rl.md) · 初读挂点
- [全身控制与执行](deepmimic/wbc.md) · 初读挂点
- [本篇方法链路](deepmimic/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
