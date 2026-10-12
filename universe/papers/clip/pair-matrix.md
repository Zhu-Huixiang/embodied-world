# 批内相似度矩阵 · CLIP

N个图像与N个文本组成N×N比较表。

U和V都是N×512，UVᵀ产生N×N分数；行是图选文本，列是文本选图。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#22-训练目标完整写一句话负担有点重)

继续拆：[正配对、负例与假负例](positive-negative.md) · [双向交叉熵](bidirectional.md) · [温度与可学习缩放](temperature.md) · [大批次与训练规模](batch-scale.md)。

[本篇星系](../clip.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md) · [原文依据](https://proceedings.mlr.press/v139/radford21a.html)
