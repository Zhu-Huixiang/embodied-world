# 仿真中的17维环境因素 · RMA

载荷质量及位置合计3维、电机强度12维、摩擦1维和局部地高1维组成训练侧环境向量。

这些值由仿真提供给环境编码器；真实部署的策略并不额外读取质量、摩擦或地形真值。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md#41-环境与动作接口)

继续拆：[局部地高压成一个标量](method-local-height.md)。

[本篇星系](../rma.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md) · [原文依据](https://www.roboticsproceedings.org/rss17/p011.pdf)
