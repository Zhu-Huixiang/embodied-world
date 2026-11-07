# 部署删未来，再缓存观测键值 · La-JEPA

预测监督留在参数里，运行时只积分动作。

移除future tokens，World时间固定0，观测各层K/V只计算一次；动作从噪声按Euler积分，默认10步。每次生成32动作，LIBERO执行10步、RoboTwin执行24步后观察并重规划。

继续拆：[0.10B可训练不等于0.10B部署](la-jepa-size.md) · [一次策略调用快，不等于机器人控制频率](la-jepa-latency.md)。

[本篇星系](../la-jepa.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/la-jepa.md) · [原文依据](https://arxiv.org/pdf/2611.08156v1)
