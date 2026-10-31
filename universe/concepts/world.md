# 世界模型

学习状态随动作或时间如何变化，用于预测、计划或训练策略。

预测对象可以是像素、latent、奖励或与决策相关的潜状态。

继续拆：[动作条件动力学](dynamics.md) · [模型预测控制 MPC](mpc.md) · [想象轨迹训练](imagination.md) · [树搜索与轨迹搜索](search.md) · [世界动作联合建模](wam.md)。

## 在完整解读里看计算与例子

- [DreamerV3：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dreamerv3-2301.04104/README.md#main别把通用算法读成同一个万能大脑)
- [MuZero：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md#1-引言会做决定得先会复刻世界吗)

## 哪些论文用到或讨论它

- [DreamerV3](../papers/dreamerv3.md) · 已精讲 · [原文](https://www.nature.com/articles/s41586-025-08744-2)
- [MuZero](../papers/muzero.md) · 已精讲 · [原文](https://www.nature.com/articles/s41586-020-03051-4)
- [SuperMimic](../papers/supermimic.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.28480)
- [world2vec](../papers/world2vec.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.40637v1)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
