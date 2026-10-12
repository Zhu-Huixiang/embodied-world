# 本篇方法链路 · TD3+BC

TD3+BC 保留 TD3 的双 Q 与 actor-critic 框架，在策略目标里同时提高 Q 值并拉近策略动作和数据动作。状态标准化稳定输入尺度，Q 值归一化的系数平衡价值追求与行为克隆。原文在 D4RL 连续控制中重跑部分基线，并报告性能与计算成本。

TD3+BC 保留 TD3 的双 Q 与 actor-critic 框架，在策略目标里同时提高 Q 值并拉近策略动作和数据动作。状态标准化稳定输入尺度，Q 值归一化的系数平衡价值追求与行为克隆。原文在 D4RL 连续控制中重跑部分基线，并报告性能与计算成本。

[本篇星系](../td3-bc.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/td3-bc.md) · [原文依据](https://proceedings.neurips.cc/paper/2021/hash/a8166da05c5a094f7dc03724b41886e5-Abstract.html)
