# 八头与输出投影 · Transformer

多个低维投影各自读取，再拼接变换。

base的8头各64维，拼接512维后乘512×512输出矩阵。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md#322-多头八组小空间一起读)

[本篇星系](../attention.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md) · [原文依据](https://arxiv.org/abs/1706.03762v7)
