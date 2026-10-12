# 残差向量量化 RVQ · VQ-BeT

用第一层码近似向量，再用后续码近似剩余误差，最后把各层码相加重建。

Holo-M 使用四级码；层级是逐次补误差，不是四个独立动作。

[跨论文技术入口](../../concepts/rvq.md)

[本篇星系](../vq-bet.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/vq-bet.md) · [原文依据](https://proceedings.mlr.press/v235/lee24y.html)
