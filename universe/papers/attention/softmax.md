# softmax 与温度 · Transformer

对候选分数取指数后归一化为总和为 1 的概率。温度控制分差如何影响概率。

温度改变概率集中程度；候选集合也会改变概率分母。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md#32-注意力qkv-分工不靠玄学)

[跨论文技术入口](../../concepts/softmax.md)

[本篇星系](../attention.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md) · [原文依据](https://papers.nips.cc/paper/2017/hash/3f5ee243547dee91fbd053c1c4a845aa-Abstract.html)
