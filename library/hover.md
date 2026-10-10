# HOVER: Versatile Neural Whole-Body Controller for Humanoid Robots

**解读导读** · ICRA 2025 · [Locomotion 与运动适应](../paper-map/README.md#track-locomotion)

研究范围：人形全身低层控制。

[原文入口](https://hover-versatile-humanoid.github.io/) · [原文 PDF](https://arxiv.org/pdf/2410.21229) · [作者项目 / 代码入口](https://hover-versatile-humanoid.github.io/) · [作者与团队](../leaderboard/origins/papers/hover.md)

ICRA 2025；不是 RSS。统一的是预设低层命令模式，不等于自动高层模式决策。

## 先看它做了什么

先训练全身 motion oracle；上/下身模式与稀疏 mask 改写任务命令，本体观测 mask 改写状态；DAgger 用 oracle 动作监督学生访问状态，得到一个统一低层策略。

## 带着什么问题读

**一个全身策略怎样接住关节、身体位置、根速度等不同格式的指令？**

## 为什么值得继续读

ICRA 2025 正式论文；oracle、命令 mask 和 DAgger 蒸馏有明确接口，仿真多模式对照与实机控制值得精选。

证据入口：模式/稀疏命令 mask 与 oracle-student DAgger；关节rad、位置mm、根速度m/s、旋转rad分项对照。（II 方法、Fig.2 / Fig.3）

具身关联：人形全身低层控制；一个全身策略怎样接住关节、身体位置、根速度等不同格式的指令？

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/hover/README.md) · [ICRA集锦](../venues/ICRA/README.md) · [地图方向](../paper-map/README.md#track-locomotion) · [首页](../README.md)

元数据核对：2026-10-10。
