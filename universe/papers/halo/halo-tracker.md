# 50Hz跟踪器处理身体与接触 · HALO

跟踪器将运动参考、本体历史和局部深度转成29个目标关节角。

48×84深度由2D CNN编码；30步本体历史与后30帧计划经1D CNN，再与当前状态和5帧前瞻拼到SimBa残差网络。输出由低层PD控制跟踪。

继续拆：[先按接触类型训练三类专家](halo-experts.md) · [机器人自己的遮挡也要进入深度](halo-depth.md) · [跟上动作还要真的推动物体](halo-contact.md) · [两台机载计算机分开语义与实时控制](halo-onboard.md)。

[本篇星系](../halo.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/halo.md) · [原文依据](https://arxiv.org/pdf/2611.06908v1)
