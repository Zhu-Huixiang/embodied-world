# 模拟器—模型—策略交替训练 · SuperMimic

真实物理模拟器产生训练转移，模型和策略在同一循环中轮流更新。

当前策略→MuJoCo Warp→回放池→世界模型拟合→模型内策略改进，循环重复。

继续拆：[回放池与8步模型拟合](replay.md) · [32步想象与时间反传](bptt.md) · [动作条件的全身跟踪](motion.md)。

[本篇星系](../supermimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/supermimic.md) · [原文依据](https://arxiv.org/pdf/2610.28480v1)
