# 奖励与旧Q组成回归目标 · CQL

Bellman备份把即时奖励与折扣后继策略价值组合成critic的训练目标。

目标动作来自当前策略，目标值来自旧Q；它不是来自新增环境执行。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md#2-预备知识高估如何钻进-bellman-目标)

继续拆：[策略评估与策略改进交替](policy-evaluation-improvement.md)。

[本篇星系](../cql.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md) · [原文依据](https://papers.nips.cc/paper_files/paper/2020/file/0d2b2061826a5df3221116a5085a6052-Paper.pdf)
