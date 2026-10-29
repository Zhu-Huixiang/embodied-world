# 行softmax权重 · Transformer

每个query对可见key获得归一化权重。

权重沿key维相加为1，AV输出的query数不变而内容维为d_v。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md#32-注意力qkv-分工不靠玄学)

[本篇星系](../attention.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md) · [原文依据](https://arxiv.org/abs/1706.03762v7)
