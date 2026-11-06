# 固定路径力矩仿射化 · cuRoboV2-Fast

路径固定后，力矩可写成速度平方及其路径导数的仿射式。

三次逆动力学求g、A+g、D+g，随后改时间无需反复完整动力学；这沿用TOPPRA等已有路径约化思想。

[本篇星系](../curobov2-fast.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/curobov2-fast.md) · [原文依据](https://arxiv.org/pdf/2611.06913v1)
