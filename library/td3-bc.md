# A Minimalist Approach to Offline Reinforcement Learning

**解读导读** · NeurIPS 2021 · [强化学习与离线决策](../paper-map/README.md#track-reinforcement-learning)

研究范围：离线 RL 基础；连续控制。

[原文入口](https://proceedings.neurips.cc/paper/2021/hash/a8166da05c5a094f7dc03724b41886e5-Abstract.html) · [原文 PDF](https://proceedings.neurips.cc/paper/2021/file/a8166da05c5a094f7dc03724b41886e5-Paper.pdf)

## 先看它做了什么

TD3+BC 保留 TD3 的双 Q 与 actor-critic 框架，在策略目标里同时提高 Q 值并拉近策略动作和数据动作。状态标准化稳定输入尺度，Q 值归一化的系数平衡价值追求与行为克隆。原文在 D4RL 连续控制中重跑部分基线，并报告性能与计算成本。

## 带着什么问题读

**只在 TD3 策略损失里加一个模仿项，为什么能成为可靠的离线 RL 基线？**

## 为什么值得继续读

用最小改动检验离线 RL 算法复杂度必要性；Cal-QL 原文继续使用 TD3+BC 作微调对照，是有复用证据的标准基础选题。

证据入口：贡献集中且容易实现；固定数据基准、基线重跑和性能/成本比较支持其基线价值，后续离线到在线研究明确复用。

具身关联：用最小改动检验离线 RL 算法复杂度必要性；Cal-QL 原文继续使用 TD3+BC 作微调对照，是有复用证据的标准基础选题。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/td3-bc/README.md) · [NeurIPS集锦](../venues/NeurIPS/README.md) · [地图方向](../paper-map/README.md#track-reinforcement-learning) · [首页](../README.md)

元数据核对：2026-10-10。
