# 三项仿真控制的收益和失败 · world2vec

world2vec改善Pendulum/Reacher，视觉CartPole仍失败。

Table1 DCL回报826/895/232，DreamerV3为668/792/899，TD-MPC2为911/744/894；最大1000。在线奖励训练、离线随机数据和控制频率不同，不能宣传全面胜出。

继续拆：[LeWM原目标到达协议](goal-protocol.md) · [复用与外推边界](limits.md)。

[本篇星系](../world2vec.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/world2vec.md) · [原文依据](https://arxiv.org/pdf/2610.40637v1)
