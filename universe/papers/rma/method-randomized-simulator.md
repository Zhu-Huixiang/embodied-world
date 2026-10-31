# 在变化的仿真动力学中练走路 · RMA

RaiSim中的A1模型配合分形不平地形和环境参数随机化产生多样行走条件。

训练与测试有不同的参数范围，并能在同一episode内重新采样条件；固定一个任务开始时的条件不足以描述这套评测。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md#41-环境与动作接口)

继续拆：[地形变化帮助学习抬脚与稳步](method-fractal-terrain.md) · [部署省适应数据不等于训练便宜](method-training-budget.md)。

[本篇星系](../rma.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md) · [原文依据](https://www.roboticsproceedings.org/rss17/p011.pdf)
