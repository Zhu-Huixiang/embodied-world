# 交叉熵 · RT-1

正确候选的负对数概率。正确项概率越小，损失越大，梯度会推动正确分数上升。

CLIP 对行和列分别计算平均交叉熵，再平均两个方向。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md#52-d-区监督的答案就是人类当时选的动作)

[跨论文技术入口](../../concepts/cross-entropy.md)

[本篇星系](../rt1.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md) · [原文依据](https://www.roboticsproceedings.org/rss19/p025.html)
