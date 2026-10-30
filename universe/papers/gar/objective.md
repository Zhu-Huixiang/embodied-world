# 动作分布的复杂度与控制代价 · GAR

检验已训练flow策略是否需要多步生成其条件动作分布。

以同一教师的完整采样、原始单步、均值读出和随机高斯读出对照；目标是保留控制能力并减少动作网络调用，而非训练新骨干。

继续拆：[固定观测下的高斯近似](gaussian-test.md) · [零时刻速度场与条件均值](mean-identity.md) · [冻结骨干的一次前向](frozen-path.md)。

[本篇星系](../gar.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/gar.md) · [原文依据](https://arxiv.org/pdf/2610.40271v1)
