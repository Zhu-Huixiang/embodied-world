# 遮挡图块预测teacher特征 · DINOv2

iBOT在student遮挡位置预测未遮挡teacher对应patch的原型分布。

iBOT保留位置对应的监督，让局部表示承担读出任务；预测对象是特征分布，不是RGB像素重建。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#43-ibot遮住局部对齐对应位置)

继续拆：[图像头和图块头分开](untied-heads.md)。

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://arxiv.org/pdf/2304.07193v2)
