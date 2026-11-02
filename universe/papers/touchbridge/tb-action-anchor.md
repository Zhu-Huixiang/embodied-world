# 固定场景坐标中的动作转换 · TouchBridge

消除头戴相机运动，否则头动会被误当作机器人动作。

另用固定场景AprilTag校正相机运动；手臂以action chunk初始帧表达相对运动，手部为绝对关节目标。

继续拆：[触觉用于离线转换而非策略输入](tb-policy.md) · [匹配初始场景下的轨迹回放](tb-replay.md)。

[本篇星系](../touchbridge.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/touchbridge.md) · [原文依据](https://arxiv.org/pdf/2610.40349v1)
