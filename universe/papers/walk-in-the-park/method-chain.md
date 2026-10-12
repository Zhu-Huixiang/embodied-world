# 本篇方法链路 · Walk in the Park

基于 SAC/DroQ 的 actor-critic 从实机回放数据学习，用较高更新比、Dropout 和归一化稳定值函数。策略直接输出关节目标，本体传感器提供状态和奖励，异步采样训练与仔细的动作空间设计减少等待。论文在室内外多种地面验证从头学走路，并在模拟中分析设计选择。

基于 SAC/DroQ 的 actor-critic 从实机回放数据学习，用较高更新比、Dropout 和归一化稳定值函数。策略直接输出关节目标，本体传感器提供状态和奖励，异步采样训练与仔细的动作空间设计减少等待。论文在室内外多种地面验证从头学走路，并在模拟中分析设计选择。

[本篇星系](../walk-in-the-park.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/walk-in-the-park.md) · [原文依据](https://www.roboticsproceedings.org/rss19/p056.html)
