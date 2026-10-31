# 随机动作视觉数据与切分 · world2vec

每环境20万帧，以完整episode分训练验证测试。

2000×100帧、1400/300/300episode；Pendulum/CartPole用OU扭矩，Reacher均匀随机。CartPole越界时还向内推，不说采集无任何环境设计。

[本篇星系](../world2vec.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/world2vec.md) · [原文依据](https://arxiv.org/pdf/2610.40637v1)
