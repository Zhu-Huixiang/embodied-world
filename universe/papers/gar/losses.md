# 三种读出目标与训练 · GAR

分别拟合均值、协方差与离散概率，保留坐标尺度。

均值最小二乘；协方差以各坐标平均目标方差归一后拟合，并加权重0.1的对数方差比误差；命令头对教师频率做BCE。协方差目标以教师经验均值居中，不用学生均值误差膨胀它。

[本篇星系](../gar.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/gar.md) · [原文依据](https://arxiv.org/pdf/2610.40271v1)
