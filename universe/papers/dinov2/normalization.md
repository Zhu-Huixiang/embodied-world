# 向量归一化 · DINOv2

把向量除以自己的 L2 长度，得到单位向量。点积随后比较方向，减少向量大小的干扰。

CLIP 两路各投影到共享空间后再归一化；B/32 示例是 N×512。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#45-koleo-与高分辨率让特征分得开也看得细)

[跨论文技术入口](../../concepts/normalization.md)

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://openreview.net/forum?id=a68SUt6zFt)
