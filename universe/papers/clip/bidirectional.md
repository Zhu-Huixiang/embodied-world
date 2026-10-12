# 双向交叉熵 · CLIP

两个检索方向的平均损失再平均。

图像选择配文与配文选择图像都要计算，行列竞争对手不同；总损失对两个方向各给一半权重。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#22-训练目标完整写一句话负担有点重)

继续拆：[梯度如何推动配对](gradient.md)。

[本篇星系](../clip.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md) · [原文依据](https://proceedings.mlr.press/v139/radford21a.html)
