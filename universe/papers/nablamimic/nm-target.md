# 定弧度动作目标 · ∇Mimic

用梯度方向指定改动作的方向，用物理量指定步幅。

y_t=a_t+δg_t/RMS(g)，δ初值.03rad并随学习率衰减；继承PODS回归思想，非所有目标回归均为本篇原创。

继续拆：[一段求导窗口复用八次回归](nm-regress.md) · [动作目标界与实际策略更新](nm-bound.md)。

[本篇星系](../nablamimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/nablamimic.md) · [原文依据](https://arxiv.org/pdf/2610.41654v1)
