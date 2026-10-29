# 预热后衰减学习率 · Transformer

前4000步线性增大，再按步数平方根倒数减小。

base还乘512的负二分之一次方，参数s表示训练步而非句子位置。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md#5-训练答案右移未来遮住)

[本篇星系](../attention.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md) · [原文依据](https://arxiv.org/abs/1706.03762v7)
