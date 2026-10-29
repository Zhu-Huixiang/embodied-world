# 闭环滚动与历史偏移 · SAM 2

重复预测、执行或生成，把新观测或模型历史接回后续计算。

Teacher forcing 与运行时自有历史之间的差异需单独检查。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam2-2408.00714/README.md#44-d-区把这次预测写进下次的条件)

[跨论文技术入口](../../concepts/rollout.md)

[本篇星系](../sam2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam2-2408.00714/README.md) · [原文依据](https://openreview.net/forum?id=Ha6RTeWMd0)
