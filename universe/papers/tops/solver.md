# 一次积分步与两次网络求值 · TOPS

用匹配时序的两半步求解动作轨迹。

one step依次调用两次速度网络，NFE=2；K=0时退化成两次Euler半步，为一阶方法，不是学得ODE的精确解。

继续拆：[源、路径和求解器的联合消融](component-ablation.md)。

[本篇星系](../tops.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/tops.md) · [原文依据](https://arxiv.org/html/2610.36694v1)
