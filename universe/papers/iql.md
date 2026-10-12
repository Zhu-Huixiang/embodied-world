# IQL 星系

Offline Reinforcement Learning with Implicit Q-Learning

**导读** · 强化学习与离线决策

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/iql.md) · [原文](https://iclr.cc/virtual/2022/poster/5941) · [评分卡](../../leaderboard/papers/iql/README.md)

IQL 在数据动作的 Q 值上做非对称 expectile 回归，拟合偏向较好动作的状态值 V。Q 用奖励加下一状态 V 做 Bellman 更新，策略再按优势加权回归数据中的动作。这个过程把值学习与策略提取拆开，实验用 D4RL 与在线微调检查拼接和改善能力。

## 技术挂点

- [离线强化学习](../concepts/offline.md)：从已有轨迹学习决策，训练时不能自由去环境补齐数据外动作的后果。

- [价值估计与校准](../concepts/value.md)：估计未来累积收益，再用保守、分位或参考价值等约束减少误导。

- [行为克隆](../concepts/bc.md)：直接监督观测到动作的映射，不必在每次更新中根据奖励搜索。

## 本篇行星与卫星

- [离线强化学习](iql/offline.md) · 初读挂点
- [价值估计与校准](iql/value.md) · 初读挂点
- [行为克隆](iql/bc.md) · 初读挂点
- [本篇方法链路](iql/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
