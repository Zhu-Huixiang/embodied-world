# 局部匹配需要距离分配与筛选 · DINOv2

patch对应先按特征欧氏距离解分配，再用非极大抑制减少连线。

Fig10展示跨风格和对象的部件关联；这项可视化还未给出3D位姿误差或机器人抓取成功率。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#75-pca-与跨图匹配)

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://arxiv.org/pdf/2304.07193v2)
