# 目标编码与CEM规划 · world2vec

用潜状态到目标的加权距离选择动作序列。

CEM采样候选、保留低成本序列并重拟合分布，执行前缀后重规划；没有奖励模型/状态解码器，仍需目标帧。

继续拆：[目标帧与Reacher逆运动学](goals.md) · [三项仿真控制的收益和失败](control-evidence.md)。

[本篇星系](../world2vec.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/world2vec.md) · [原文依据](https://arxiv.org/pdf/2610.40637v1)
