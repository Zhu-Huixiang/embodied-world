# 防止策略只抄本体或依赖一个相机 · La-JEPA

丢条件、视觉增强与观测编码器LoRA共同构成最终配方。

文字、本体、相机dropout各0.1；LIBERO任一相机可丢，RoboTwin只丢腕相机，至少留一视角。只增强观测；LoRA适配观测编码器，未来监督始终用冻结编码器的干净存储特征。

继续拆：[适配观测并不要求目标也随之漂移](la-jepa-targets.md)。

[本篇星系](../la-jepa.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/la-jepa.md) · [原文依据](https://arxiv.org/pdf/2611.08156v1)
