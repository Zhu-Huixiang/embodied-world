# 用仿真真值编码监督适应器 · RMA

第二阶段把环境编码器输出作为目标，以预测潜变量与目标的平方误差训练适应器。

环境编码器和基础策略已固定；只更新适应器参数。部署不需要这个真值目标，也不运行该监督学习更新。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md#32-适应模块从半秒经历估计控制条件)

继续拆：[让训练历史包含自己的失误](method-on-policy-history.md)。

[本篇星系](../rma.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md) · [原文依据](https://www.roboticsproceedings.org/rss17/p011.pdf)
