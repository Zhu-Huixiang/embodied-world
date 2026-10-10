# Learning to Walk in Minutes Using Massively Parallel Deep Reinforcement Learning

**解读导读** · CoRL 2021 · [Locomotion 与运动适应](../paper-map/README.md#track-locomotion)

研究范围：腿足 RL 的训练基础设施与 sim-to-real。

[原文入口](https://proceedings.mlr.press/v164/rudin22a.html) · [原文 PDF](https://proceedings.mlr.press/v164/rudin22a/rudin22a.pdf) · [作者项目 / 代码入口](https://leggedrobotics.github.io/legged_gym/)

CoRL 2021；PMLR 164 论文集出版年为 2022。

## 先看它做了什么

物理仿真和 PPO 训练都留在 GPU 上，用大量并行环境快速组成更新批次。地形课程根据机器人前进表现升降难度，任务课程逐步扩大命令范围。原文分析大并行下训练组件并把 ANYmal 策略转到实机，公开 legged_gym。

## 带着什么问题读

**把几千只机器人放到同一块 GPU，训练速度与课程怎么一起改变？**

## 为什么值得继续读

legged_gym 路线的代表基础论文；大并行训练、课程和实机迁移共同支撑后续腿足控制工作，不只是算得快。

证据入口：有训练设置分析、课程与 sim-to-real 实验；公开代码是复用入口，后续 Extreme Parkour 原文直接比较该工作。

具身关联：legged_gym 路线的代表基础论文；大并行训练、课程和实机迁移共同支撑后续腿足控制工作，不只是算得快。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/walk-in-minutes/README.md) · [CoRL集锦](../venues/CoRL/README.md) · [地图方向](../paper-map/README.md#track-locomotion) · [首页](../README.md)

元数据核对：2026-10-10。
