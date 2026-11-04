# 把参考速度放回阻尼项 · CR-DAgger

追踪运动轨迹时，不能把所有阻尼都用于压住机器人速度。

扩展稿使用D(qdot_ref−qdot)替代−D qdot，以减少运动参考下的跟踪落后。该改变服务微小纠正标签的方向准确性。

继续拆：[给纠正标签补偿硬件延迟](cr-latency.md)。

[本篇星系](../cr-dagger.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/cr-dagger.md) · [原文依据](https://compliant-residual-dagger.github.io/files/CR_DAgger_extended.pdf)
