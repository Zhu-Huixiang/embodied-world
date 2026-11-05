# 让高Q动作成为惩罚候选 · CQL

Eq3在候选分布上最大化Q并用正则限制提案。

候选分布暴露当前价值函数的乐观部分，外层critic再压低它。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md#32-离线策略学习用-log-sum-exp-找到虚高动作)

继续拆：[CQL(H)的软最大值](logsumexp.md) · [前一策略先验的ρ变体](cql-rho.md)。

[本篇星系](../cql.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md) · [原文依据](https://papers.nips.cc/paper_files/paper/2020/file/0d2b2061826a5df3221116a5085a6052-Paper.pdf)
