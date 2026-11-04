# 约50Hz推理的力感知残差策略 · CR-DAgger

残差补充快而小的接触修正。

输入冻结的视觉表征、状态和力历史；推理循环约50Hz，每次预测5个0.02s动作、覆盖0.1s。预测时域0.1s不等于推理循环10Hz；导纳执行循环另为500Hz。

继续拆：[时间卷积读取接触力历史](cr-force-encoder.md) · [15维动作与目标力/力矩](cr-action.md) · [残差头结构不是唯一解释](cr-architecture.md)。

[本篇星系](../cr-dagger.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/cr-dagger.md) · [原文依据](https://compliant-residual-dagger.github.io/files/CR_DAgger_extended.pdf)
