# 回放池与8步模型拟合 · SuperMimic

用模拟器记录的状态和动作监督未来状态预测。

一次读取k=8的自回归窗口，后续预测接着使用模型自己的前一步状态；世界模型并非只做单步回归。

继续拆：[随机化环境上下文](context.md)。

[本篇星系](../supermimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/supermimic.md) · [原文依据](https://arxiv.org/pdf/2610.28480v1)
