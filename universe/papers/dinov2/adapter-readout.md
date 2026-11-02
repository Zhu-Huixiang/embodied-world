# 冻结骨干外面仍可接复杂解码器 · DINOv2

ViT-Adapter与Mask2Former可训练而ViT-g保持固定，得到更强分割输出。

ADE20k60.2 mIoU来自这个更复杂读出系统；只冻结了66%权重，不能用它替代简单linear的比较。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#74-分割与深度)

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://arxiv.org/pdf/2304.07193v2)
