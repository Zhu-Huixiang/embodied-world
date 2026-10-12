# TD3+BC 星系

A Minimalist Approach to Offline Reinforcement Learning

**导读** · 强化学习与离线决策

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/td3-bc.md) · [原文](https://proceedings.neurips.cc/paper/2021/hash/a8166da05c5a094f7dc03724b41886e5-Abstract.html) · [评分卡](../../leaderboard/papers/td3-bc/README.md)

TD3+BC 保留 TD3 的双 Q 与 actor-critic 框架，在策略目标里同时提高 Q 值并拉近策略动作和数据动作。状态标准化稳定输入尺度，Q 值归一化的系数平衡价值追求与行为克隆。原文在 D4RL 连续控制中重跑部分基线，并报告性能与计算成本。

## 技术挂点

- [离线强化学习](../concepts/offline.md)：从已有轨迹学习决策，训练时不能自由去环境补齐数据外动作的后果。

- [策略与价值学习](../concepts/actor-critic.md)：actor 产生动作，critic 估计长期收益；价值估计为策略改进提供方向。

- [行为克隆](../concepts/bc.md)：直接监督观测到动作的映射，不必在每次更新中根据奖励搜索。

## 本篇行星与卫星

- [离线强化学习](td3-bc/offline.md) · 初读挂点
- [策略与价值学习](td3-bc/actor-critic.md) · 初读挂点
- [行为克隆](td3-bc/bc.md) · 初读挂点
- [本篇方法链路](td3-bc/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
