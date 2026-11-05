# 策略评估与策略改进交替 · CQL

critic估计策略回报，actor提高高价值动作的概率。

保守校准进入critic目标，随后通过actor的Q目标影响选择。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md#41-图-d-怎样接住修正后的-q)

[本篇星系](../cql.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md) · [原文依据](https://papers.nips.cc/paper_files/paper/2020/file/0d2b2061826a5df3221116a5085a6052-Paper.pdf)
