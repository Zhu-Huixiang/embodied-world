# 从局部token读出像素类别 · DINOv2

linear头把patch向量映成类别logit，低分辨率logit图再上采样。

+ms另叠最后四层、640分辨率与多尺度测试；ADE20k的49.0 linear和53.0 +ms是不同设置。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#74-分割与深度)

继续拆：[冻结骨干外面仍可接复杂解码器](adapter-readout.md)。

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://arxiv.org/pdf/2304.07193v2)
