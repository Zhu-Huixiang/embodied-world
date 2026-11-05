# CQL(H)的软最大值 · CQL

logsumexp平滑聚合所有动作价值，高Q动作在其梯度里占较大权重。

减去数据Q之后，动作梯度是softmax概率与数据动作频率之差。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md#32-离线策略学习用-log-sum-exp-找到虚高动作)

继续拆：[一升一降来自概率之差](regularizer-gradient.md)。

[本篇星系](../cql.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md) · [原文依据](https://papers.nips.cc/paper_files/paper/2020/file/0d2b2061826a5df3221116a5085a6052-Paper.pdf)
