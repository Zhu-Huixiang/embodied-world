# 模型内树搜索 · MuZero

在隐藏状态上试分支，环境只执行最后选择的动作。

每条边缓存N/Q/P/R/S，重复访问复用模型结果。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md#34-一次搜索挑路扩一格往回记账)

继续拆：[pUCT选择](puct.md) · [叶节点扩张](expand.md) · [折扣回传与均值](backup.md) · [访问次数转策略](visits.md) · [根合法动作与内部模型](legal.md)。

[本篇星系](../muzero.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md) · [原文依据](https://arxiv.org/pdf/1911.08265v2)
