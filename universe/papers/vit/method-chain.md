# 本篇方法链路 · ViT

将图像切成固定大小的 patch，每块展平后线性投影为 token，再加入位置编码送进标准 Transformer。原文以大规模监督预训练和小规模下游微调测试数据规模与视觉归纳偏置的关系。实验覆盖 ImageNet、CIFAR 和 VTAB，机器人中的视觉 backbone 是这条表示路线的后续应用。

将图像切成固定大小的 patch，每块展平后线性投影为 token，再加入位置编码送进标准 Transformer。原文以大规模监督预训练和小规模下游微调测试数据规模与视觉归纳偏置的关系。实验覆盖 ImageNet、CIFAR 和 VTAB，机器人中的视觉 backbone 是这条表示路线的后续应用。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/vit-2010.11929/README.md#3-方法这张图到底怎样穿过-transformer)

[本篇星系](../vit.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/vit-2010.11929/README.md) · [原文依据](https://iclr.cc/virtual/2021/poster/3013)
