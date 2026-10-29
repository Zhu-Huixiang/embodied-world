# 冻结未来目标分支 · JAM

记录的未来观测只在训练目标分支编码。

冻结anchor输出按时间偏移对齐的目标token；stop-gradient阻断目标分支更新，未来不进入动作输入路径。

继续拆：[当前token预测未来特征](head.md) · [未来目标取什么表征](targets.md) · [缓存后的在线训练成本](cost.md)。

[本篇星系](../jam.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/jam.md) · [原文依据](https://arxiv.org/html/2610.37219v1)
