# HOVER 星系

HOVER: Versatile Neural Whole-Body Controller for Humanoid Robots

**导读** · Locomotion 与运动适应

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/hover.md) · [原文](https://hover-versatile-humanoid.github.io/) · [评分卡](../../leaderboard/papers/hover/README.md)

先训练全身 motion oracle；上/下身模式与稀疏 mask 改写任务命令，本体观测 mask 改写状态；DAgger 用 oracle 动作监督学生访问状态，得到一个统一低层策略。

## 技术挂点

- [教师学生蒸馏](../concepts/distill.md)：用教师的预测或动作监督学生，让部署模型复制可用行为。

- [遮蔽预测](../concepts/masking.md)：隐藏部分输入，训练模型恢复像素、token 或表征。恢复什么决定监督重点。

- [全身控制与执行](../concepts/wbc.md)：将运动目标、机器人状态和约束转成关节目标或力矩，协调腿、手臂与底盘。

## 本篇行星与卫星

- [教师学生蒸馏](hover/distill.md) · 初读挂点
- [遮蔽预测](hover/masking.md) · 初读挂点
- [全身控制与执行](hover/wbc.md) · 初读挂点
- [本篇方法链路](hover/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
