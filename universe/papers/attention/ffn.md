# 逐位置前馈层 · Transformer

每个位置独立地变换通道特征。

512→2048→512，中间ReLU；同层跨位置共享权重，但此子层本身不交换位置内容。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md#33-前馈层交换信息后每个位置再自己加工)

[本篇星系](../attention.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md) · [原文依据](https://arxiv.org/abs/1706.03762v7)
