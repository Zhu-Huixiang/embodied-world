# 线性探测 · CLIP

冻结编码器，用带标签的下游样本训练线性预测头，以检查特征本身是否容易迁移。

要分清读取投影前特征还是归一化图文向量。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#33-表征换个分类头才能单独看视觉底子)

[跨论文技术入口](../../concepts/linear-probe.md)

[本篇星系](../clip.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md) · [原文依据](https://proceedings.mlr.press/v139/radford21a.html)
