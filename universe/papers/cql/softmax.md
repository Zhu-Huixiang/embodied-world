# softmax 与温度 · CQL

对候选分数取指数后归一化为总和为 1 的概率。温度控制分差如何影响概率。

温度改变概率集中程度；候选集合也会改变概率分母。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md#32-离线策略学习用-log-sum-exp-找到虚高动作)

[跨论文技术入口](../../concepts/softmax.md)

[本篇星系](../cql.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md) · [原文依据](https://proceedings.neurips.cc/paper_files/paper/2020/hash/0d2b2061826a5df3221116a5085a6052-Abstract.html)
