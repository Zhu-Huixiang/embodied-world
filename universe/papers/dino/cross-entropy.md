# 交叉熵 · DINO

正确候选的负对数概率。正确项概率越小，损失越大，梯度会推动正确分数上升。

CLIP 对行和列分别计算平均交叉熵，再平均两个方向。

[跨论文技术入口](../../concepts/cross-entropy.md)

[本篇星系](../dino.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dino.md) · [原文依据](https://openaccess.thecvf.com/content/ICCV2021/html/Caron_Emerging_Properties_in_Self-Supervised_Vision_Transformers_ICCV_2021_paper.html)
