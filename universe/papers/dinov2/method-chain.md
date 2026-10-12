# 本篇方法链路 · DINOv2

在大规模筛选图像上扩展图像级与 patch 级自监督学习，再把大 ViT 教师蒸馏为不同尺寸的编码器。下游可以冻结 backbone，用轻量预测头读取分类、分割或深度相关信息。原文比较多种图像与像素任务；OpenVLA 的视觉输入实际将 DINOv2 特征与 SigLIP 特征拼接后映射给语言模型。

在大规模筛选图像上扩展图像级与 patch 级自监督学习，再把大 ViT 教师蒸馏为不同尺寸的编码器。下游可以冻结 backbone，用轻量预测头读取分类、分割或深度相关信息。原文比较多种图像与像素任务；OpenVLA 的视觉输入实际将 DINOv2 特征与 SigLIP 特征拼接后映射给语言模型。

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dinov2.md) · [原文依据](https://openreview.net/forum?id=a68SUt6zFt)
