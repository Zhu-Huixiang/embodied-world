# PPO 与并行模拟

用受约束的策略更新与大量模拟轨迹训练控制；并行度改变每轮数据和训练开销。

GPU 同驻留减少数据来回搬运，但不改变奖励设计的责任。

分类上层：[强化学习](rl.md)。

## 在完整解读里看计算与例子

- [RMA：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md#42-网络与训练预算)

## 哪些论文用到或讨论它

- [RMA](../papers/rma.md) · 已精讲 · [原文](https://www.roboticsproceedings.org/rss17/p011.html)
- [Legged Gym](../papers/walk-in-minutes.md) · 机制导读 · [原文](https://proceedings.mlr.press/v164/rudin22a.html)
- [SONIC](../papers/sonic.md) · 机制导读 · [原文](https://www.science.org/doi/10.1126/scirobotics.aed4592)
- [Isaac Gym](../papers/isaac-gym.md) · 机制导读 · [原文](https://datasets-benchmarks-proceedings.neurips.cc/paper/2021/hash/28dd2c7955ce926456240b2ff0100bde-Abstract-round2.html)
- [DiffContact](../papers/diffcontact.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.35852v1)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
