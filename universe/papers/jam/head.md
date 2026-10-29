# 当前token预测未来特征 · JAM

训练期小预测头把当前token映射到未来目标空间。

两层token-mixing transformer和每offset线性readout；Wan/Ovis头宽1536/768，余弦损失在token和时间偏移上平均。

继续拆：[动作损失与预见损失](loss.md) · [删除训练期分支](deploy.md)。

[本篇星系](../jam.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/jam.md) · [原文依据](https://arxiv.org/html/2610.37219v1)
