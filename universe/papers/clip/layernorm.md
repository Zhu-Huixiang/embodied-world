# LayerNorm · CLIP

对一条特征内部的数值做均值和方差归一化。

LayerNorm在编码器内部稳定特征尺度；投影后的L2归一化把整个向量长度压成1，二者位置和目的不同。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#23-模型两边各自干活最后才对答案)

[本篇星系](../clip.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md) · [原文依据](https://proceedings.mlr.press/v139/radford21a.html)
