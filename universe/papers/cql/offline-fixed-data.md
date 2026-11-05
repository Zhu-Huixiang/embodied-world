# 固定数据里的策略改进 · CQL

只用历史状态动作奖励转移训练策略，学习过程中不追加环境交互。

离线仍能进行许多梯度更新和候选动作查询，但不能把这些查询当成新试验。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md#1-引言封存的数据开放的动作想象)

继续拆：[虚高估值的自举反馈](bootstrap-ood-loop.md) · [训练动作偏移与执行状态偏移](state-action-shift.md)。

[本篇星系](../cql.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md) · [原文依据](https://papers.nips.cc/paper_files/paper/2020/file/0d2b2061826a5df3221116a5085a6052-Paper.pdf)
