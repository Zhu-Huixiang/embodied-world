# 残差向量量化 RVQ · Holo-M

用第一层码近似向量，再用后续码近似剩余误差，最后把各层码相加重建。

Holo-M 使用四级码；层级是逐次补误差，不是四个独立动作。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md#31-统一动作编码208究竟怎么算出来的)

[跨论文技术入口](../../concepts/rvq.md)

[本篇星系](../holo-m.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md) · [原文依据](https://arxiv.org/abs/2609.35709v1)
