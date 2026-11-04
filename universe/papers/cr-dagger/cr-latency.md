# 给纠正标签补偿硬件延迟 · CR-DAgger

用实际姿态减去延迟对齐的参考姿态，避免把控制误差当纠正。

q_delta[t]=q[t]−q_ref[t−Delta t]；Delta t依具体硬件标定。大于纠正量的跟踪落后会翻转标签符号。

[本篇星系](../cr-dagger.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/cr-dagger.md) · [原文依据](https://compliant-residual-dagger.github.io/files/CR_DAgger_extended.pdf)
