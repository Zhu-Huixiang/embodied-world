# 先共同训练策略与环境编码器 · RMA

第一阶段通过PPO联合优化基础策略与环境编码器，使压缩后的条件对行走有用。

强化学习优化的是期望折扣回报；编码器不是独立拟合物理标签，环境因素经它进入策略，控制结果反过来塑造表示。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md#31-基础策略特权信息怎样教出一套步态)

继续拆：[向前走之外还要付运动代价](method-natural-reward.md)。

[本篇星系](../rma.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md) · [原文依据](https://www.roboticsproceedings.org/rss17/p011.pdf)
