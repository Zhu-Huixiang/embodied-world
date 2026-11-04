# 动作目标界与实际策略更新 · ∇Mimic

裁剪和批RMS共同限制每个目标偏移。

每样本每关节RMS目标偏移≤sqrt(2)κδ≈.1273rad；界作用于监督目标，神经策略优化不自动获得严格信赖域保证。

[本篇星系](../nablamimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/nablamimic.md) · [原文依据](https://arxiv.org/pdf/2610.41654v1)
