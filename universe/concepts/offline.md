# 离线强化学习

从已有轨迹学习决策，训练时不能自由去环境补齐数据外动作的后果。

数据覆盖与值函数外推决定策略是否敢选不可靠动作。

分类上层：[强化学习](rl.md)。

继续拆：[价值估计与校准](value.md)。

## 哪些论文用到或讨论它

- [robomimic](../papers/robomimic.md) · 机制导读 · [原文](https://proceedings.mlr.press/v164/mandlekar22a.html)
- [IQL](../papers/iql.md) · 机制导读 · [原文](https://iclr.cc/virtual/2022/poster/5941)
- [TD3+BC](../papers/td3-bc.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper/2021/hash/a8166da05c5a094f7dc03724b41886e5-Abstract.html)
- [Decision Transformer](../papers/decision-transformer.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2021/hash/7f489f642a0ddb10272b5c31057f0663-Abstract.html)
- [Cal-QL](../papers/cal-ql.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2023/hash/c44a04289beaf0a7d968a94066a1d696-Abstract-Conference.html)
- [CQL](../papers/cql.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2020/hash/0d2b2061826a5df3221116a5085a6052-Abstract.html)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
