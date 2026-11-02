# 图像头和图块头分开 · DINOv2

图像CLS目标与patch目标使用独立MLP投影头。

头权重分开避免把两种目标的映射硬绑在一起；作者是在规模化设置中观察其效果，不声称这是所有规模的定理。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#43-ibot遮住局部对齐对应位置)

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://arxiv.org/pdf/2304.07193v2)
