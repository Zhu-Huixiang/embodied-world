# 32步想象与时间反传 · SuperMimic

沿可微模型展开H=32步，把后续奖励对当前动作的导数传回策略。

策略更新内固定模型参数，但仍保留对状态和动作的梯度；接触模拟器本身不参与微分。

继续拆：[末端价值与短段想象](critic.md)。

[本篇星系](../supermimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/supermimic.md) · [原文依据](https://arxiv.org/pdf/2610.28480v1)
