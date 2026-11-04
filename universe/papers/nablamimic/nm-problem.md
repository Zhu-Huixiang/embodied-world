# 接触动力学为何让一阶策略学习爆炸 · ∇Mimic

把跟踪奖励沿动力学求导本可省样本，但接触切换使少数样本导数极大。

论文将问题分成梯度尾部失控与求导成本，而非宣布所有世界模型都无用。

继续拆：[G1全身动作跟踪](nm-task.md) · [短窗回报与价值自举](nm-objective.md) · [同轨迹精确与模型梯度比较](nm-tail.md) · [单机器人融合求导引擎](nm-engine.md)。

[本篇星系](../nablamimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/nablamimic.md) · [原文依据](https://arxiv.org/pdf/2610.41654v1)
