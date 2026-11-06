# 没有物体，怎样学会施力 · Ctrl-F

训练时施加指令力的反向外力，让机器人维持参考姿态。

随机采样f并对指定刚体施加−f；保持运动跟踪奖励。学到的力条件响应在物体接触中使用，不要求低层输入物体模型或成对交互示范。稳态力平衡是训练直觉，不是所有动态接触的精确力跟踪保证。

继续拆：[负载掩码限定能施力的身体](cf-mask.md) · [先跟稳，再逐步增加指令力](cf-curriculum.md) · [零力条件下仍可跟踪动作](cf-zero-load.md) · [只改指令，外力轨迹保持一致](cf-command-test.md)。

[本篇星系](../ctrl-f.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/ctrl-f.md) · [原文依据](https://arxiv.org/pdf/2611.05507v1)
