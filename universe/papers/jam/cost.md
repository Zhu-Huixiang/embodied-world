# 缓存后的在线训练成本 · JAM

提前提取固定未来目标，减少每次更新的目标计算。

Wan估算FLOPs为15.52→4.19 TFLOPs/sample/update；所profile算子GPU时间0.789→0.258秒，不含一次提取，也省略部分算子与优化器成本。

[本篇星系](../jam.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/jam.md) · [原文依据](https://arxiv.org/html/2610.37219v1)
