# 多相机、本体与指令各走哪条路 · La-JEPA

视觉进入World DiT，文字和本体成为两路DiT的条件。

V-JEPA 2.1 ViT-L逐相机编码；FLAN-T5-large冻结编码文字，本体经学习投影为token；两DiT通过交叉注意力读条件，另有独立注意力投影和前馈层。

继续拆：[当前两帧与未来十六帧分开编码](la-jepa-tube.md) · [动作看观测，不直接看未来token](la-jepa-mask.md) · [防止策略只抄本体或依赖一个相机](la-jepa-robustness.md)。

[本篇星系](../la-jepa.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/la-jepa.md) · [原文依据](https://arxiv.org/pdf/2611.08156v1)
