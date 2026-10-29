# 编码器解码器堆叠 · Transformer

编码源句，依据目标前缀逐步输出。

原版base有6层encoder与6层decoder，每层主表示512维。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md#31-编码器与解码器两列各六层)

继续拆：[残差后LayerNorm](post-ln.md) · [逐位置前馈层](ffn.md) · [词嵌入和缩放](embedding.md)。

[本篇星系](../attention.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md) · [原文依据](https://arxiv.org/abs/1706.03762v7)
