# 动作条件动力学

以当前状态和动作预测下一状态或分布，建立“做这个动作会发生什么”的计算接口。

不能把无动作的视频预测直接当成可干预的动力学。

分类上层：[世界模型](world.md)。

继续拆：[逆动力学](inverse.md)。

## 在完整解读里看计算与例子

- [MuZero：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md#32-hgf各自接什么吐什么)

## 哪些论文用到或讨论它

- [Dreamer](../papers/dreamer.md) · 机制导读 · [原文](https://research.google/pubs/dream-to-control-learning-behaviors-by-latent-imagination/)
- [DreamerV2](../papers/dreamerv2.md) · 机制导读 · [原文](https://research.google/pubs/mastering-atari-with-discrete-world-models/)
- [DreamerV3](../papers/dreamerv3.md) · 机制导读 · [原文](https://www.nature.com/articles/s41586-025-08744-2)
- [TD-MPC](../papers/td-mpc.md) · 机制导读 · [原文](https://proceedings.mlr.press/v162/hansen22a.html)
- [TD-MPC2](../papers/td-mpc2.md) · 机制导读 · [原文](https://proceedings.iclr.cc/paper_files/paper/2024/hash/cf73d57b6dcda32b293df7c2d5341f49-Abstract-Conference.html)
- [EfficientZero](../papers/efficientzero.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper/2021/hash/d5eca8dc3820cad9fe56a3bafda65ca1-Abstract.html)
- [EfficientZero V2](../papers/efficientzero-v2.md) · 机制导读 · [原文](https://proceedings.mlr.press/v235/wang24at.html)
- [DayDreamer](../papers/daydreamer.md) · 机制导读 · [原文](https://proceedings.mlr.press/v205/wu23c.html)
- [MuZero](../papers/muzero.md) · 已精讲 · [原文](https://www.nature.com/articles/s41586-020-03051-4)
- [ASAP](../papers/asap.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss21/p066.html)
- [LeWM](../papers/lewm.md) · 机制导读 · [原文](https://arxiv.org/abs/2603.19312v1)
- [Ctrl-World](../papers/ctrl-world.md) · 机制导读 · [原文](https://proceedings.iclr.cc/paper_files/paper/2026/hash/0ae94013da7cd459402fd77874e09ee3-Abstract-Conference.html)
- [Dynamics Review](../papers/learned-dynamics-review.md) · 机制导读 · [原文](https://www.science.org/doi/10.1126/scirobotics.adt1497)
- [V-JEPA 2](../papers/vjepa2.md) · 机制导读 · [原文](https://arxiv.org/abs/2506.09985)
- [SuperMimic](../papers/supermimic.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.28480)
- [DiffContact](../papers/diffcontact.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.35852v1)
- [DreamTrue](../papers/dreamtrue.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.12468v1)
- [LeWAM](../papers/lewam.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.12407v1)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
