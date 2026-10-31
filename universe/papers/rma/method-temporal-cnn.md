# 时间卷积提取动作响应模式 · RMA

每步42维状态与动作先映射到32维，再由三层一维卷积沿时间提取关联。

论文给出的卷积输入/输出通道均为32，核宽与步长依次为8/4、5/1、5/1；展平后线性映射为8维条件。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md#42-网络与训练预算)

[本篇星系](../rma.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md) · [原文依据](https://www.roboticsproceedings.org/rss17/p011.pdf)
