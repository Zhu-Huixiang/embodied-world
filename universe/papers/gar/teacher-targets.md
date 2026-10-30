# 教师采样目标与数据划分 · GAR

从已部署教师采样估计经验均值、协方差与命令频率。

Human300每任务5示范×4状态，合6000拟合context；600调参与600矩评估context来自各自独立示范。每context384教师样本构建目标；协方差向对角收缩5%并做特征值下限。

继续拆：[三种读出目标与训练](losses.md) · [0.02%状态背后的准备成本](preparation.md)。

[本篇星系](../gar.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/gar.md) · [原文依据](https://arxiv.org/pdf/2610.40271v1)
