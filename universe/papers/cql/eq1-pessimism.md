# Eq1：候选动作整体受压 · CQL

在Bellman误差上增加候选分布下Q期望的最小化。

候选分布也可能包含数据里的好动作；全部下压易损失价值尺度，因此下一步加入数据支撑项。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md#31-保守策略评估从逐项下压到期望下界)

继续拆：[Eq2：数据动作托住价值](eq2-data-support.md)。

[本篇星系](../cql.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md) · [原文依据](https://papers.nips.cc/paper_files/paper/2020/file/0d2b2061826a5df3221116a5085a6052-Paper.pdf)
