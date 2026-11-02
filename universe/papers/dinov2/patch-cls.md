# 一个整图token和一组局部token · DINOv2

ViT将图像分块编码，CLS用于整图读出，patch token保留位置对应的局部特征。

224方形输入和patch14对应256个patch，加CLS共257个token；ViT-g特征宽1536，维度是从论文设置展开的计算。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#41-图像怎样变成-token)

继续拆：[跨裁切匹配整图分布](dino-image-loss.md) · [遮挡图块预测teacher特征](ibot-patch-loss.md) · [末段提高图像分辨率](high-res-tail.md)。

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://arxiv.org/pdf/2304.07193v2)
