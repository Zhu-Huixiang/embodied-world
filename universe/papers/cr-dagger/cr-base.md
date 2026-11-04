# 冻结低频扩散基策略 · CR-DAgger

保留学好的大幅运动，让新数据只学局部改正。

基策略推理循环约1Hz，每次预测32个未来末端目标，动作间隔0.1s、预测跨度3.2s；循环频率与预测时域分别记录，基础策略保持冻结。

继续拆：[约50Hz推理的力感知残差策略](cr-residual.md)。

[本篇星系](../cr-dagger.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/cr-dagger.md) · [原文依据](https://compliant-residual-dagger.github.io/files/CR_DAgger_extended.pdf)
