# 把动作当成一个视频patch · TAPESTRY

将每个动作先对齐视频VAE的patch输入，再复用预训练tokenizer。

20维动作经64×20矩阵、无仿射LayerNorm形成2×2×16伪patch；同一个预训练patchifier把它送入DiT，一个时刻只用一个token。

继续拆：[复用视频输出层和转置读出](readout.md)。

[本篇星系](../tapestry.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/tapestry.md) · [原文依据](https://arxiv.org/pdf/2610.36823v1)
