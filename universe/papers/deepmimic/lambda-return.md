# 多步与λ回报 · DeepMimic

已观察奖励加后继value组成n步目标，再以λ加权不同n。

TDλ训练critic；有限轨迹结尾的终止条件决定是否自举。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md#4-背景奖励怎样改掉下一次动作)

继续拆：[GAE把回报变为相对优势](gae-advantage.md)。

[本篇星系](../deepmimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md) · [原文依据](https://xbpeng.github.io/projects/DeepMimic/DeepMimic_2018.pdf)
