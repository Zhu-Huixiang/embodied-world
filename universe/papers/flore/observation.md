# 图像、14维状态与wrench历史 · FLoRe

高层策略观察视觉、相对本体状态和双手接触量。

两张224×224腕图经CLIP初始化ViT-B/16；相对位置、手姿和夹爪宽度组成14维状态，wrench历史用因果卷积编码。

继续拆：[运动与力的联合扩散输出](method-diffusion.md)。

[本篇星系](../flore.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/flore.md) · [原文依据](https://arxiv.org/html/2610.35862v1)
