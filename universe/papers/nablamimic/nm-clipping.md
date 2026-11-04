# 反传内逐样本中位数裁剪 · ∇Mimic

在单个巨梯度污染批平均前缩小它。

每个反向时间步对动作cotangent按κ×批中位范数裁剪，κ=3；结束再裁窗口动作梯度。保持方向但引入偏差。

继续拆：[定弧度动作目标](nm-target.md)。

[本篇星系](../nablamimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/nablamimic.md) · [原文依据](https://arxiv.org/pdf/2610.41654v1)
