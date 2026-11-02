# 无标签训练仍可能有地域偏差 · DINOv2

预训练数据的地域与收入分布会影响下游识别，各组均值并未自动相同。

DollarStreet Table12 DINOv2非洲74.0欧洲89.7，低收入67.4高收入90.5；表内差距用于具体描述，不套用原文段落的错误差值。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#8-公平性覆盖面扩大以后差距仍在哪里)

继续拆：[有害标签测试有指定集合和阈值](association-test.md)。

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://arxiv.org/pdf/2304.07193v2)
