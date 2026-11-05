# 策略期望下界 · CQL

CQL的较紧形式对目标策略加权Q的均值保守，而非对每一个动作都低估。

μ取目标策略时得到非负分布偏离项；有采样误差还需足够惩罚余量。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md#31-保守策略评估从逐项下压到期望下界)

继续拆：[CQL分布差是非负平方和](cql-divergence.md) · [慢策略更新保留保守余量](slow-policy.md)。

[本篇星系](../cql.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md) · [原文依据](https://papers.nips.cc/paper_files/paper/2020/file/0d2b2061826a5df3221116a5085a6052-Paper.pdf)
