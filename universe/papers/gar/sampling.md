# 一步采样与闭式似然 · GAR

一次动作网络前向后直接采样动作块，无速度积分。

连续动作从N(μ,Σ)抽取，离散命令从独立伯努利抽取；高斯密度乘各伯努利概率是闭式似然，可给其他候选动作打分而不再次调用网络。

继续拆：[两教师与两仿真基准](control.md) · [动作网络次数与全策略延迟](latency.md) · [单峰动作与多路径闭环行为](feedback-diversity.md)。

[本篇星系](../gar.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/gar.md) · [原文依据](https://arxiv.org/pdf/2610.40271v1)
