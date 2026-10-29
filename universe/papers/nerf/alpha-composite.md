# 前向alpha合成 · NeRF

每段按T_i alpha_i加权RGB。

alpha=1-exp(-sigma delta)，权重并非简单平均。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/nerf-2003.08934/README.md#41-连续积分怎样落到离散采样)

[本篇星系](../nerf.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/nerf-2003.08934/README.md) · [原文依据](https://arxiv.org/abs/2003.08934v2)
