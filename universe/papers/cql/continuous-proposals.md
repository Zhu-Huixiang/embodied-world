# 连续动作的二路采样 · CQL

每个数据状态从uniform和当前策略各采十个动作。

候选仅输入critic估值，不调用环境，不产生新奖励或新后继状态。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md#42-连续动作无穷多个怎么求和)

继续拆：[对候选密度作重要性校正](importance-correction.md)。

[本篇星系](../cql.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md) · [原文依据](https://papers.nips.cc/paper_files/paper/2020/file/0d2b2061826a5df3221116a5085a6052-Supplemental.pdf)
