# 本篇方法链路 · Legged Gym

物理仿真和 PPO 训练都留在 GPU 上，用大量并行环境快速组成更新批次。地形课程根据机器人前进表现升降难度，任务课程逐步扩大命令范围。原文分析大并行下训练组件并把 ANYmal 策略转到实机，公开 legged_gym。

物理仿真和 PPO 训练都留在 GPU 上，用大量并行环境快速组成更新批次。地形课程根据机器人前进表现升降难度，任务课程逐步扩大命令范围。原文分析大并行下训练组件并把 ANYmal 策略转到实机，公开 legged_gym。

[本篇星系](../walk-in-minutes.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/walk-in-minutes.md) · [原文依据](https://proceedings.mlr.press/v164/rudin22a.html)
