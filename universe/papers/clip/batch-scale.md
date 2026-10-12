# 大批次与训练规模 · CLIP

批内竞争项随批大小增加，相似度表按N²增长。

32,768对样本对应约10.74亿个配对分数；32个epoch、模型与设备账单要和样本效率区分。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#24-预训练损失短账单可不短)

[本篇星系](../clip.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md) · [原文依据](https://proceedings.mlr.press/v139/radford21a.html)
