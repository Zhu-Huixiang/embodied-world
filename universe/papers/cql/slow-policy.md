# 慢策略更新保留保守余量 · CQL

理论要求新策略接近由当前Q导出的softmax策略。

策略差异造成的潜在高估需要被保守余量覆盖，学习率不是可随意放大的无关参数。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md#32-离线策略学习用-log-sum-exp-找到虚高动作)

[本篇星系](../cql.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md) · [原文依据](https://papers.nips.cc/paper_files/paper/2020/file/0d2b2061826a5df3221116a5085a6052-Paper.pdf)
