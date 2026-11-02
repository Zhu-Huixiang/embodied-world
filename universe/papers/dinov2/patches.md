# 视觉 patch token · DINOv2

把图像切成块，展平并投影成向量，再加入位置信息。

CLIP B/32 的 224×224 图像得到 49 个图块，加 CLS 共 50 个视觉位置。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#41-图像怎样变成-token)

[跨论文技术入口](../../concepts/patches.md)

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://openreview.net/forum?id=a68SUt6zFt)
