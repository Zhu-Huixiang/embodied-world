# 目标分布适配的代价 · CLIP

让分类边界适合ImageNet，收益未必均匀迁移。

固定CLIP特征再拟合ImageNet线性头，常规准确率升高，但R、ObjectNet与Sketch得分下降。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#34-换场景香蕉一变成素描就不认识了)

[本篇星系](../clip.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md) · [原文依据](https://proceedings.mlr.press/v139/radford21a.html)
