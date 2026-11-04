# 回放起点与当前策略采样 · ∇Mimic

独立collector以噪声当前策略采样FIFO状态，按回报分箱reset。

继承SHAC/SuperMimic等数据链路；去replay改连续窗口还提高.018–.019，不能宣称replay是本篇必需创新。

[本篇星系](../nablamimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/nablamimic.md) · [原文依据](https://arxiv.org/pdf/2610.41654v1)
