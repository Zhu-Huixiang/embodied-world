# Learning to Walk in Minutes Using Massively Parallel Deep Reinforcement Learning

出处：CoRL 2021。研究范围：腿足 RL 的训练基础设施与 sim-to-real。

[原文入口](https://proceedings.mlr.press/v164/rudin22a.html) · [原文 PDF](https://proceedings.mlr.press/v164/rudin22a/rudin22a.pdf) · [作者项目 / 代码入口](https://leggedrobotics.github.io/legged_gym/)

CoRL 2021；PMLR 164 论文集出版年为 2022。

阅读问题：**把几千只机器人放到同一块 GPU，训练速度与课程怎么一起改变？**

收录理由：legged_gym 路线的代表基础论文；大并行训练、课程和实机迁移共同支撑后续腿足控制工作，不只是算得快。

证据入口：有训练设置分析、课程与 sim-to-real 实验；公开代码是复用入口，后续 Extreme Parkour 原文直接比较该工作。

具身关联：legged_gym 路线的代表基础论文；大并行训练、课程和实机迁移共同支撑后续腿足控制工作，不只是算得快。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/walk-in-minutes/README.md)

机制简析：物理仿真和 PPO 训练都留在 GPU 上，用大量并行环境快速组成更新批次。地形课程根据机器人前进表现升降难度，任务课程逐步扩大命令范围。原文分析大并行下训练组件并把 ANYmal 策略转到实机，公开 legged_gym。
<!-- discovery:end -->
