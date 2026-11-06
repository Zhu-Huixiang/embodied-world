# 路径短不等于执行快 · cuRoboV2-Fast

规划耗时和机器人实际运动耗时是两项不同目标。

负载改变动力学约束；较短关节路径可能必须走得更慢。论文同时减少优化开销和轨迹执行时间。

继续拆：[与早期cuRobo分开核身份](fast-lineage.md) · [先直线、必要时RRT再精修](fast-pipeline.md) · [接触成功成为剩余瓶颈](fast-limit.md)。

[本篇星系](../curobov2-fast.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/curobov2-fast.md) · [原文依据](https://arxiv.org/pdf/2611.06913v1)
