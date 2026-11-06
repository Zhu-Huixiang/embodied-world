# 从高斯噪声推向运动参考 · HALO

流匹配训练预测噪声到干净计划的速度。

令x1为标准化运动、x0为高斯噪声，s取Beta(1.5,1)，xs=sx1+(1−s)x0，速度目标x1−x0。逐帧DiT输出36维速度；推理以15步Euler积分。

继续拆：[把已承诺的半秒作为干净前缀](halo-prefix.md) · [流模型与回归的差异含RTC兼容性](halo-decoder-ablation.md)。

[本篇星系](../halo.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/halo.md) · [原文依据](https://arxiv.org/pdf/2611.06908v1)
