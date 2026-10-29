# 三种注意力来源 · Transformer

自注意力与交叉注意力的Q/K/V来源不同。

encoder自注意力全来自源，decoder自注意力来自目标前缀，交叉Q来自decoder而K/V来自encoder。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md#323-三种注意力来源要分清)

继续拆：[因果掩码](causal-mask.md)。

[本篇星系](../attention.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md) · [原文依据](https://arxiv.org/abs/1706.03762v7)
