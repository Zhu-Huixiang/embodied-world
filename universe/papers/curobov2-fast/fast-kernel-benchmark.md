# 模块时延不等于完整规划 · cuRoboV2-Fast

Panda7DoF/G1 29DoF、batch1与1024分别比较内核中位时间。

主规划基准仍是Panda；不能从G1计算速度推出人形任务成功。优化迭代可重叠内核，分项时间不直接求和当wall-clock。

[本篇星系](../curobov2-fast.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/curobov2-fast.md) · [原文依据](https://arxiv.org/pdf/2611.06913v1)
