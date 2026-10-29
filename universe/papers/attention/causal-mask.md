# 因果掩码 · Transformer

禁止目标位置读取未来目标。

训练时矩阵能并行计算，但未来logit先屏蔽，不能把完整标签偷偷泄漏给当前预测。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md#323-三种注意力来源要分清)

[本篇星系](../attention.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md) · [原文依据](https://arxiv.org/abs/1706.03762v7)
