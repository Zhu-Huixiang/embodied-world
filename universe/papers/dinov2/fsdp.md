# 分片训练状态 · DINOv2

student、teacher与优化器状态在多个GPU间分片，降低单卡驻留负担。

骨干权重广播和梯度归约用float16，投影头梯度float32稳定训练；训练成本与最终推理成本分开。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#51-计算工程怎样改变可训练规模)

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://arxiv.org/pdf/2304.07193v2)
