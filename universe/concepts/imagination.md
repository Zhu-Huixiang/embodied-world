# 想象轨迹训练

在学到的动力学里滚动状态，用预测奖励和值训练策略，从而增加决策训练数据。

模型误差会影响训练信号，真实反馈仍用于更新世界模型。

分类上层：[世界模型](world.md)。

## 哪些论文用到或讨论它

- [Dreamer](../papers/dreamer.md) · 机制导读 · [原文](https://research.google/pubs/dream-to-control-learning-behaviors-by-latent-imagination/)
- [DreamerV2](../papers/dreamerv2.md) · 机制导读 · [原文](https://research.google/pubs/mastering-atari-with-discrete-world-models/)
- [DreamerV3](../papers/dreamerv3.md) · 机制导读 · [原文](https://www.nature.com/articles/s41586-025-08744-2)
- [DayDreamer](../papers/daydreamer.md) · 机制导读 · [原文](https://proceedings.mlr.press/v205/wu23c.html)
- [SuperMimic](../papers/supermimic.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.28480)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
