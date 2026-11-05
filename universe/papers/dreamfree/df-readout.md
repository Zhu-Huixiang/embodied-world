# 64个可学习动作查询 · DreamFree

把可变数量视觉token压成固定动作条件。

两块self/cross-attention更新64个query，输出1024维视觉context，与投影后的指令token拼接供动作DiT交叉注意力；不经过蒸馏projector。

[本篇星系](../dreamfree.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamfree.md) · [原文依据](https://arxiv.org/pdf/2611.04527v1)
