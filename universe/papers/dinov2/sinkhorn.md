# 批内原型分配的归一化 · DINOv2

teacher使用三轮Sinkhorn-Knopp得到目标分布，student端用softmax。

它替代teacher的softmax-centering环节；不能把SK与旧EMA-centering画成必须串联的两次处理。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#44-ema-与-sinkhorn目标怎样跟着学又不挤成一团)

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://arxiv.org/pdf/2304.07193v2)
