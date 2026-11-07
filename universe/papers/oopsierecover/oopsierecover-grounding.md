# 从语言对象落到三维点集 · OopsieRecover

VLM为相关实体给出图像中的二维种子点，并判断实体用区域还是单点。

区域种子交给分割模型，区域像素经深度投影为3D点集；单点直接提升。每帧跟踪语义区域并重新采点，避免逐点跟踪漂移。

继续拆：[让模型看实体怎么动，而非整段点云](oopsierecover-centroids.md) · [何时介入与怎样改动作分开](oopsierecover-cost.md) · [换场景先重新找同一类实体](oopsierecover-transfer.md)。

[本篇星系](../oopsierecover.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/oopsierecover.md) · [原文依据](https://arxiv.org/pdf/2611.08462v1)
