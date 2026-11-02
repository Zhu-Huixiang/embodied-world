# 先去重再扩展覆盖 · DINOv2

近重复检测在图像相似度图上保留连通分量代表，并去掉与评测数据过近的图像。

附录使用近邻图和连通分量去重；相对参考数据的去重减少直接复制带来的虚高，但不等于排除全部目标域先验。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#3-数据处理样本变多之前先看覆盖有没有变)

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://arxiv.org/pdf/2304.07193v2)
