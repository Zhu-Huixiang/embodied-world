# 线性投影与共同空间 · CLIP

用可学习矩阵把两路特征映射到同一维度。

B/32中视觉投影768×512、文本投影512×512；两路最终都是512维，才可以逐对点积。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#22-训练目标完整写一句话负担有点重)

[本篇星系](../clip.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md) · [原文依据](https://proceedings.mlr.press/v139/radford21a.html)
