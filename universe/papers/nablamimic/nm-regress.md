# 一段求导窗口复用八次回归 · ∇Mimic

昂贵导数算一次，策略用多个小批次靠近同一目标。

每窗口8次16384样本Adam回归，独立优化器lr6e-4。去多步回归后绝对动作.806对.855，残差.822对.866。

[本篇星系](../nablamimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/nablamimic.md) · [原文依据](https://arxiv.org/pdf/2610.41654v1)
