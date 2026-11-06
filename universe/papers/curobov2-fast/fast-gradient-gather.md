# 按控制点收集梯度 · cuRoboV2-Fast

每个控制点只收集其局部支持范围内的样本梯度。

warp归约避免重叠样本原子累加，也不显式建样本×控制点中间张量；这是计算实现收益。

[本篇星系](../curobov2-fast.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/curobov2-fast.md) · [原文依据](https://arxiv.org/pdf/2611.06913v1)
