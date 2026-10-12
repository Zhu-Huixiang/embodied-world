# 温度与可学习缩放 · CLIP

正缩放系数改变概率集中程度。

分数乘exp(t)，温度τ=exp(−t)；方向相同的分数排名不变，softmax概率会变。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#22-训练目标完整写一句话负担有点重)

[本篇星系](../clip.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md) · [原文依据](https://proceedings.mlr.press/v139/radford21a.html)
