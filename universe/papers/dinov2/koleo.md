# 让同批特征保持展开 · DINOv2

对单位化CLS取最近邻距离的负对数平均，距离越小惩罚越大。

正则只在每块GPU内首个global crop的样本之间计算，权重0.1；它没有直接要求人为类别均匀分布。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#45-koleo-与高分辨率让特征分得开也看得细)

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://arxiv.org/pdf/2304.07193v2)
