# 交叉熵 · SAM 2

正确候选的负对数概率。正确项概率越小，损失越大，梯度会推动正确分数上升。

CLIP 对行和列分别计算平均交叉熵，再平均两个方向。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam2-2408.00714/README.md#45-e-区训练时怎样教它别跟丢)

[跨论文技术入口](../../concepts/cross-entropy.md)

[本篇星系](../sam2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam2-2408.00714/README.md) · [原文依据](https://openreview.net/forum?id=Ha6RTeWMd0)
