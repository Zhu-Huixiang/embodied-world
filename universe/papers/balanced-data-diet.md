# Balanced Data Diet 星系

A Balanced Data Diet: Addressing the Exploration Bottleneck in Mega-Scale RL for Robot Control

**导读** · Locomotion 与运动适应

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/balanced-data-diet.md) · [原文](https://arxiv.org/abs/2610.12465v1) · [评分卡](../../leaderboard/papers/balanced-data-diet/README.md)

Success Guided Sampling 根据当前成功率把重置分布推向能力边缘，减少超简单或暂时学不会的采样，再蒸馏视觉操作策略转实机。

## 技术挂点

- [机器人数据与评测](../concepts/data.md)：统一观测、动作、任务与评测条件，判断数据多样性如何影响泛化。

- [强化学习](../concepts/rl.md)：通过奖励和值评估改进策略，研究动作如何改变长期回报。

- [教师学生蒸馏](../concepts/distill.md)：用教师的预测或动作监督学生，让部署模型复制可用行为。

## 本篇行星与卫星

- [机器人数据与评测](balanced-data-diet/data.md) · 初读挂点
- [强化学习](balanced-data-diet/rl.md) · 初读挂点
- [教师学生蒸馏](balanced-data-diet/distill.md) · 初读挂点
- [本篇方法链路](balanced-data-diet/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
