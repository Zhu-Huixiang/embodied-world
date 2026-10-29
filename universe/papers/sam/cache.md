# 可缓存图像编码 · SAM

重编码图像只做一次，后续提示复用特征。

1024×1024图像经ViT-H/16与卷积颈部得到64×64×256网格。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam-2304.02643/README.md#31-a-区大图压成一张可反复查询的特征地图)

继续拆：[视觉块与空间网格](patch.md) · [MAE预训练](mae.md)。

[本篇星系](../sam.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam-2304.02643/README.md) · [原文依据](https://arxiv.org/abs/2304.02643v1)
