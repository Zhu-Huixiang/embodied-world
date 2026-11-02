# 用冻结巨型teacher训练小模型 · DINOv2

小模型训练阶段把ViT-g固定，student学习其分布，最终使用student EMA。

移除遮挡和stochastic depth，但iBOT损失仍在两个global crops上使用；不能把小模型蒸馏画成仅CLS监督。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#52-蒸馏时教师的更新规则变了)

继续拆：[蒸馏优势看同结构对照](distill-evidence.md)。

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://arxiv.org/pdf/2304.07193v2)
