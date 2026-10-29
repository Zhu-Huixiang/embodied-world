# 闭环滚动与历史偏移 · MuZero

重复预测、执行或生成，把新观测或模型历史接回后续计算。

Teacher forcing 与运行时自有历史之间的差异需单独检查。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md#34-一次搜索挑路扩一格往回记账)

[跨论文技术入口](../../concepts/rollout.md)

[本篇星系](../muzero.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md) · [原文依据](https://www.nature.com/articles/s41586-020-03051-4)
