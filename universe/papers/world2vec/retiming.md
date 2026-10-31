# 改变积分步长与控制频率 · world2vec

固定模型通过更小Euler步在更高频率规划。

同一Reacher模型10Hz训练，50Hz积分、每两步持一动作而25Hz重规划；903与952是同起点目标的一例episode回报，不当跨任务统计泛化。

[本篇星系](../world2vec.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/world2vec.md) · [原文依据](https://arxiv.org/pdf/2610.40637v1)
