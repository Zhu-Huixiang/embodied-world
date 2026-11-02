# 靠视觉检索整理训练集 · DINOv2

利用已整理图像域提供查询，从海量图像池检索相关但更多样的图像。

视觉检索器是ImageNet22k自监督训练的ViT-H/16。没有类别预测损失与没有数据域先验是不同主张。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#3-数据处理样本变多之前先看覆盖有没有变)

继续拆：[先去重再扩展覆盖](deduplication.md) · [大图像域逐样本取近邻](sample-retrieval.md) · [小数据域按簇扩充并封顶](cluster-retrieval.md) · [预训练、检索种子与评测分开](dataset-roles.md)。

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://arxiv.org/pdf/2304.07193v2)
