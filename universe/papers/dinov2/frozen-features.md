# 冻结视觉骨干的目标 · DINOv2

预训练后的图像编码器保持参数不变，图像级和图块级输出支持不同视觉任务。

冻结表示降低每个下游任务改动大骨干的需要；分类、分割和深度头仍从各自任务标签学习。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#1-引言一套特征能不能少为每个任务重练一次)

继续拆：[配文与像素信息的取舍](caption-detail.md)。

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://arxiv.org/pdf/2304.07193v2)
