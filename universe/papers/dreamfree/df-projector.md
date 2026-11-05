# 从当前token扩展未来token · DreamFree

对齐头把当前表示变成教师时空布局。

复制N个当前token到F个时间位置，加可学习帧嵌入；两层decoder做自注意力、向当前token交叉注意力和1024→4096→1024 MLP。

继续拆：[未来token余弦蒸馏](df-distill.md)。

[本篇星系](../dreamfree.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamfree.md) · [原文依据](https://arxiv.org/pdf/2611.04527v1)
