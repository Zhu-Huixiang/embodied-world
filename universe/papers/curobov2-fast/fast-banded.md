# 局部支持带来的带状Newton系统 · cuRoboV2-Fast

每个约束样本关联四个时间控制点。

primal–dual预测与校正复用一次Cholesky分解，回溯保留可行步，并保存最短可行迭代；不是凸全局最优证明。

[本篇星系](../curobov2-fast.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/curobov2-fast.md) · [原文依据](https://arxiv.org/pdf/2611.06913v1)
