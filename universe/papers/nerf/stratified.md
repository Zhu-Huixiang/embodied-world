# 分层随机采样 · NeRF

每个等距区间抽一个点，覆盖射线范围。

训练不同随机落点使连续函数不只在固定网格上被查询。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/nerf-2003.08934/README.md#41-连续积分怎样落到离散采样)

[本篇星系](../nerf.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/nerf-2003.08934/README.md) · [原文依据](https://arxiv.org/abs/2003.08934v2)
