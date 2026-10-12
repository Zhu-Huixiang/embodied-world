# 交叉熵 · CLIP

正确候选的负对数概率。正确项概率越小，损失越大，梯度会推动正确分数上升。

CLIP 对行和列分别计算平均交叉熵，再平均两个方向。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#22-训练目标完整写一句话负担有点重)

继续拆：[softmax 与温度](softmax.md)。

[跨论文技术入口](../../concepts/cross-entropy.md)

[本篇星系](../clip.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md) · [原文依据](https://proceedings.mlr.press/v139/radford21a.html)
