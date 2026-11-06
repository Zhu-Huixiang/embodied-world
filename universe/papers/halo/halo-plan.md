# 五秒运动写成150乘36 · HALO

每帧包含29关节角、3维骨盆位移和4维骨盆四元数。

150帧对应30Hz下5秒；位移和朝向相对于当前骨盆坐标，关节角和位移按维标准化，四元数保持原值。生成的是运动学参考，关节电机命令由跟踪器另算。

继续拆：[从高斯噪声推向运动参考](halo-flow.md)。

[本篇星系](../halo.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/halo.md) · [原文依据](https://arxiv.org/pdf/2611.06908v1)
