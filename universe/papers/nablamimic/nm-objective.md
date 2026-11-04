# 短窗回报与价值自举 · ∇Mimic

有限时间反传可控制开销，窗外收益交给critic。

4096个H=64的窗口；稠密跟踪奖励加γ^H末端价值，γ=.99；TDλ=.95。

继续拆：[反传内逐样本中位数裁剪](nm-clipping.md) · [梯度链长度与critic依赖](nm-horizon.md) · [回放起点与当前策略采样](nm-replay.md) · [终止屏蔽与训练跌倒惩罚](nm-fall.md)。

[本篇星系](../nablamimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/nablamimic.md) · [原文依据](https://arxiv.org/pdf/2610.41654v1)
