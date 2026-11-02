# 大图像域逐样本取近邻 · DINOv2

ImageNet22k和GLDv2每图检索4张近邻，ImageNet1k train每图检索32张。

这一配额使后者构成重要来源。最终集还含ImageNet22k等直接加入的图像，不能把全部142M描述为统一每图取4近邻。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#3-数据处理样本变多之前先看覆盖有没有变)

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://arxiv.org/pdf/2304.07193v2)
