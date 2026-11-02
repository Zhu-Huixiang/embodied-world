# 主成分颜色展示部件关联 · DINOv2

先用首主成分阈值去背景，再对相关图的前景patch共同做PCA并将前三分量映成RGB。

同组相关部件呈相近颜色是定性现象；颜色不是语义真值，也不是跨任意PCA组通用的类别编码。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#75-pca-与跨图匹配)

继续拆：[局部匹配需要距离分配与筛选](patch-assignment.md)。

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://arxiv.org/pdf/2304.07193v2)
