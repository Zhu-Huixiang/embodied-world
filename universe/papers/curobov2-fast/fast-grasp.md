# 抓取与转移分两次规划 · cuRoboV2-Fast

IK先从候选抓取姿态中选择，再生成连接运动。

第一调用规划pregrasp、直线approach和lift；第二调用规划transfer。IK可行不能保证路径可达，接触许可按阶段配置。

继续拆：[五物体模拟抓放](fast-simulation.md) · [YAM实机感知与抓取集成](fast-real-system.md)。

[本篇星系](../curobov2-fast.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/curobov2-fast.md) · [原文依据](https://arxiv.org/pdf/2611.06913v1)
