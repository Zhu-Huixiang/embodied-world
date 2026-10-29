# 策略与价值学习

actor 产生动作，critic 估计长期收益；价值估计为策略改进提供方向。

在真实或想象轨迹上训练，会面对不同的误差来源。

分类上层：[强化学习](rl.md)。

## 在完整解读里看计算与例子

- [DreamerV3：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dreamerv3-2301.04104/README.md#critic-learning只想十六步怎么惦记更远的钻石)

## 哪些论文用到或讨论它

- [Dreamer](../papers/dreamer.md) · 机制导读 · [原文](https://research.google/pubs/dream-to-control-learning-behaviors-by-latent-imagination/)
- [DreamerV3](../papers/dreamerv3.md) · 已精讲 · [原文](https://www.nature.com/articles/s41586-025-08744-2)
- [TD3+BC](../papers/td3-bc.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper/2021/hash/a8166da05c5a094f7dc03724b41886e5-Abstract.html)
- [Cal-QL](../papers/cal-ql.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2023/hash/c44a04289beaf0a7d968a94066a1d696-Abstract-Conference.html)
- [CQL](../papers/cql.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2020/hash/0d2b2061826a5df3221116a5085a6052-Abstract.html)
- [Bipedal Soccer](../papers/bipedal-soccer.md) · 机制导读 · [原文](https://www.science.org/doi/10.1126/scirobotics.adi8022)
- [Walk in the Park](../papers/walk-in-the-park.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss19/p056.html)
- [SuperMimic](../papers/supermimic.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.28480)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
