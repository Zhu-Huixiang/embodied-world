# 一层跟动作，一层发力指令 · Ctrl-F

低层输出全身关节位置目标，高层为每个指定接触刚体输出三维力。

低层输入机器人参考运动、力指令与本体状态；高层还读取物体参考运动、接触点和测得物体状态。先训低层再冻结，高层通过物体偏差调整指令。

继续拆：[没有物体，怎样学会施力](cf-inverse.md) · [从物体误差决定该多用多少力](cf-force-planner.md) · [九种任务对应三套策略对](cf-families.md)。

[本篇星系](../ctrl-f.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/ctrl-f.md) · [原文依据](https://arxiv.org/pdf/2611.05507v1)
