# 15维动作与目标力/力矩 · CR-DAgger

动作同时说明往哪里改、想施加多少力。

每步9维SE(3)位姿表示加6维wrench（3维力与3维力矩）；位姿增量和目标力/力矩分别进入顺应执行，不只预测位置残差。

继续拆：[500Hz控制闭环接住两种动作](cr-execution.md)。

[本篇星系](../cr-dagger.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/cr-dagger.md) · [原文依据](https://compliant-residual-dagger.github.io/files/CR_DAgger_extended.pdf)
