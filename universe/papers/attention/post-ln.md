# 残差后LayerNorm · Transformer

先加子层输出，再对通道做归一化。

原版是Post-LN；保留残差信息路径并控制通道数值尺度，不混作后来的Pre-LN。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md#31-编码器与解码器两列各六层)

[本篇星系](../attention.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md) · [原文依据](https://arxiv.org/abs/1706.03762v7)
