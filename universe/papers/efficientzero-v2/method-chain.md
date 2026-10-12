# 本篇方法链路 · EfficientZero V2

表示函数得到潜状态，动力学函数接收动作并预测潜状态与奖励，策略和值网络为搜索提供先验。连续动作下先采样候选动作，再用基于 Gumbel 的树搜索改善策略，并用搜索产生价值目标以利用旧经验。实验按有限交互预算比较离散和连续、图像和低维输入任务。

表示函数得到潜状态，动力学函数接收动作并预测潜状态与奖励，策略和值网络为搜索提供先验。连续动作下先采样候选动作，再用基于 Gumbel 的树搜索改善策略，并用搜索产生价值目标以利用旧经验。实验按有限交互预算比较离散和连续、图像和低维输入任务。

[本篇星系](../efficientzero-v2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/efficientzero-v2.md) · [原文依据](https://proceedings.mlr.press/v235/wang24at.html)
