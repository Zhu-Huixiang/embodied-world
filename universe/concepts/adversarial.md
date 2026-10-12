# 对抗动作模仿

判别器区分参考与策略运动，将判别信号转成鼓励符合参考风格的奖励。

这类先验约束动作分布，不等于每帧必须跟随同一参考。

分类上层：[动作先验](motion-prior.md)。

## 哪些论文用到或讨论它

- [AMP](../papers/amp.md) · 机制导读 · [原文](https://xbpeng.github.io/projects/AMP/)
- [ASE](../papers/ase.md) · 机制导读 · [原文](https://xbpeng.github.io/projects/ASE/)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
