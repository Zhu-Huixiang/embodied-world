# 参考姿态加关节残差 · ∇Mimic

初始策略先跟参考，学习修正而非从零生成姿态。

残差版.34h到.82，绝对动作.50h；动作率惩罚施加在最终指令setpoint，保持奖励定义一致。

[本篇星系](../nablamimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/nablamimic.md) · [原文依据](https://arxiv.org/pdf/2610.41654v1)
