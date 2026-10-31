# 让训练历史包含自己的失误 · RMA

训练rollout由适应器预测的条件驱动基础策略，而不是始终喂完美环境条件。

随机初始化和不准确预测会把机器人带到非理想状态；在这些轨迹上继续监督适应器，使它学习处理部署时也会遇到的偏离。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md#32-适应模块从半秒经历估计控制条件)

[本篇星系](../rma.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md) · [原文依据](https://www.roboticsproceedings.org/rss17/p011.pdf)
