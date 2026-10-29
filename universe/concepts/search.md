# 树搜索与轨迹搜索

展开候选动作或轨迹，用预测价值挑选可执行方案。

MuZero 在潜状态中做 MCTS；轨迹 Transformer 用 beam search。

分类上层：[世界模型](world.md)。

## 在完整解读里看计算与例子

- [MuZero：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md#34-一次搜索挑路扩一格往回记账)

## 哪些论文用到或讨论它

- [EfficientZero](../papers/efficientzero.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper/2021/hash/d5eca8dc3820cad9fe56a3bafda65ca1-Abstract.html)
- [EfficientZero V2](../papers/efficientzero-v2.md) · 机制导读 · [原文](https://proceedings.mlr.press/v235/wang24at.html)
- [Trajectory Transformer](../papers/trajectory-transformer.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2021/hash/099fe6b0b444c23836c4a5d07346082b-Abstract.html)
- [Diffuser](../papers/diffuser.md) · 机制导读 · [原文](https://proceedings.mlr.press/v162/janner22a.html)
- [MuZero](../papers/muzero.md) · 已精讲 · [原文](https://www.nature.com/articles/s41586-020-03051-4)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
