# Offline Reinforcement Learning with Implicit Q-Learning

**解读导读** · ICLR 2022 · [强化学习与离线决策](../paper-map/README.md#track-reinforcement-learning)

研究范围：离线 RL 基础；操作和导航数据学习。

[原文入口](https://iclr.cc/virtual/2022/poster/5941) · [原文 PDF](https://arxiv.org/pdf/2110.06169) · [作者项目 / 代码入口](https://github.com/ikostrikov/implicit_q_learning) · [作者与团队](../leaderboard/origins/papers/iql.md)

按 ICLR 2022 正式录用版本归档；arXiv 首稿为 2021。

## 先看它做了什么

IQL 在数据动作的 Q 值上做非对称 expectile 回归，拟合偏向较好动作的状态值 V。Q 用奖励加下一状态 V 做 Bellman 更新，策略再按优势加权回归数据中的动作。这个过程把值学习与策略提取拆开，实验用 D4RL 与在线微调检查拼接和改善能力。

## 带着什么问题读

**从未评价数据外动作，IQL 为什么还能拼接次优轨迹并改善策略？**

## 为什么值得继续读

离线 RL 的标准基线路线；Trajectory Transformer 与 Cal-QL 原文直接拿它比较或使用其 Q 函数，适合讲清分布偏移与轨迹拼接。

证据入口：算法简洁、公开实现，多域离线基准及微调实验；后续正式论文把它作为比较对象与 Q 引导组件，复用证据明确。

具身关联：离线 RL 的标准基线路线；Trajectory Transformer 与 Cal-QL 原文直接拿它比较或使用其 Q 函数，适合讲清分布偏移与轨迹拼接。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/iql/README.md) · [ICLR集锦](../venues/ICLR/README.md) · [地图方向](../paper-map/README.md#track-reinforcement-learning) · [首页](../README.md)

元数据核对：2026-10-10。
