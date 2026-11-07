# 数据回放成功和关节连续性先过关 · La-JEPA

训练过滤与评测模拟器选择会改变结果。

LIBERO用MuJoCo3.3.2，回放2000演示保留1777；对齐本体时刻并按1st/99th百分位缩放。RoboTwin2500clean演示排除62条跨±π关节不连续路径，保留2438条。

继续拆：[同一指令协议下比较小模型](la-jepa-libero.md) · [clean学到的技能在随机场景剩多少](la-jepa-robotwin.md)。

[本篇星系](../la-jepa.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/la-jepa.md) · [原文依据](https://arxiv.org/pdf/2611.08156v1)
