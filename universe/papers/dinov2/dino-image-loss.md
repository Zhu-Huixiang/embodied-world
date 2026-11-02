# 跨裁切匹配整图分布 · DINOv2

DINO头把CLS映成原型概率，student去匹配同图其他裁切的teacher分布。

交叉熵的目标是teacher软分布，不是人工类别名；预训练投影头与后续分类头用途不同。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#42-dino不同裁剪对齐整图判断)

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://arxiv.org/pdf/2304.07193v2)
