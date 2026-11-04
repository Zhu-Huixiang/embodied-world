# 接触解最优条件的隐式求导 · ∇Mimic

通过约束解的条件求导，避免回放所有Newton迭代。

离散接触集、active set和clamp决策固定；Newton10步与implicitfast。它是当前离散步局部导数，不是穿越所有接触切换的全局光滑梯度。

继续拆：[精确模式与训练导数规则](nm-guards.md) · [有限差分校验导数](nm-accuracy.md)。

[本篇星系](../nablamimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/nablamimic.md) · [原文依据](https://arxiv.org/pdf/2610.41654v1)
