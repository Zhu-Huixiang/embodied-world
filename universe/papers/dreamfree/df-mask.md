# 当前帧可见性约束 · DreamFree

训练时输入未来帧，不让当前帧表征偷看未来。

当前token在视频自注意力中只看当前；每个未来latent帧只看当前与自身，未来token禁用文本交叉注意力，帧内空间注意力保留。

[本篇星系](../dreamfree.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamfree.md) · [原文依据](https://arxiv.org/pdf/2611.04527v1)
