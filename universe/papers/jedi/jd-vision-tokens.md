# 视觉patch输入与预测目标的维度 · JEDI

示范图像编码和未来预测目标来自不同编码器，token数和通道宽度分别计算。

示范侧SigLIP So400m/14冻结并缓存：8个采样帧×2个视角×每图256个patch token，共4096个视觉token，每个宽1152；另有128步状态/动作的MLP嵌入，不计入这4096个视觉token。查询侧SigLIP在训练时微调。未来关键帧目标来自冻结V-JEPA2.1 ViT-L的两帧clip，输出256个宽1024的patch token；这不是SigLIP通道宽度。

[本篇星系](../jedi.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/jedi.md) · [原文依据](https://arxiv.org/pdf/2610.40356v1)
