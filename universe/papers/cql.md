# CQL 星系

Conservative Q-Learning for Offline Reinforcement Learning

**导读** · 强化学习与离线决策

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/cql.md) · [原文](https://proceedings.neurips.cc/paper_files/paper/2020/hash/0d2b2061826a5df3221116a5085a6052-Abstract.html) · [评分卡](../../leaderboard/papers/cql/README.md)

CQL 在 Bellman 误差外增加正则：压低策略或广泛采样动作的 Q 值，相对抬高数据动作的 Q 值。得到的保守值函数用于策略改进，从而减少数据外动作被过高估计的风险。原文同时给出值下界分析、离散与连续控制实验及复杂数据分布比较。

## 技术挂点

- [离线强化学习](../concepts/offline.md)：从已有轨迹学习决策，训练时不能自由去环境补齐数据外动作的后果。

- [价值估计与校准](../concepts/value.md)：估计未来累积收益，再用保守、分位或参考价值等约束减少误导。

- [策略与价值学习](../concepts/actor-critic.md)：actor 产生动作，critic 估计长期收益；价值估计为策略改进提供方向。

## 本篇行星与卫星

- [离线强化学习](cql/offline.md) · 初读挂点
- [价值估计与校准](cql/value.md) · 初读挂点
- [策略与价值学习](cql/actor-critic.md) · 初读挂点
- [本篇方法链路](cql/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
