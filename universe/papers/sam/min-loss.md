# 多候选最小损失 · SAM

含糊输入选择误差最小的候选更新掩码分支。

三个候选计算20倍focal加Dice；取最小分支，避免强迫每次只押一种粒度。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam-2304.02643/README.md#34-d-区三个答案怎么训练不会全长成一样吗)

继续拆：[IoU与质量预测](iou.md) · [模拟交互训练](interactive-train.md)。

[本篇星系](../sam.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam-2304.02643/README.md) · [原文依据](https://arxiv.org/abs/2304.02643v1)
