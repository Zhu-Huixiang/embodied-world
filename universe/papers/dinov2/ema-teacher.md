# 参数平均产生缓慢teacher · DINOv2

teacher由student参数的指数滑动平均更新，不用同一交叉熵再直接反传。

每步结束更新，动量从0.994余弦升至1。目标变化比即时student缓慢；固定大teacher蒸馏是后续另一阶段。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#44-ema-与-sinkhorn目标怎样跟着学又不挤成一团)

继续拆：[批内原型分配的归一化](sinkhorn.md)。

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://arxiv.org/pdf/2304.07193v2)
