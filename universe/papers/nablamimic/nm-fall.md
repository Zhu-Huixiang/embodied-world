# 终止屏蔽与训练跌倒惩罚 · ∇Mimic

在达到硬终止前给可微风险信号。

v1保留survival mask并对高度/倾斜加平滑训练惩罚，评测不加此项；整套移除变化<.01。当前项目稿已改窗口终止处理，须与v1分开。

[本篇星系](../nablamimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/nablamimic.md) · [原文依据](https://arxiv.org/pdf/2610.41654v1)
