# 小数据域按簇扩充并封顶 · DINOv2

图像池分为十万簇，从小种子集覆盖的簇抽样，再限制每个数据域的最终数量。

图像池分为十万簇，按查询覆盖选簇再采样，为小数据域限制最终取样量，避免某次检索主导整体配比。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#3-数据处理样本变多之前先看覆盖有没有变)

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://arxiv.org/pdf/2304.07193v2)
