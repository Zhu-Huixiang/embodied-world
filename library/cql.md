# Conservative Q-Learning for Offline Reinforcement Learning

**解读导读** · NeurIPS 2020 · [强化学习与离线决策](../paper-map/README.md#track-reinforcement-learning)

研究范围：离线 RL 基础；机器人静态数据学习。

[原文入口](https://proceedings.neurips.cc/paper_files/paper/2020/hash/0d2b2061826a5df3221116a5085a6052-Abstract.html) · [原文 PDF](https://papers.nips.cc/paper_files/paper/2020/file/0d2b2061826a5df3221116a5085a6052-Paper.pdf)

经典例外；正式 NeurIPS 2020。

## 先看它做了什么

CQL 在 Bellman 误差外增加正则：压低策略或广泛采样动作的 Q 值，相对抬高数据动作的 Q 值。得到的保守值函数用于策略改进，从而减少数据外动作被过高估计的风险。原文同时给出值下界分析、离散与连续控制实验及复杂数据分布比较。

## 带着什么问题读

**离线数据没有覆盖的动作，怎样避免被 Q 函数凭空吹成好动作？**

## 为什么值得继续读

保守离线 RL 基础方法，TD3+BC、IQL、DT、Trajectory Transformer 和 Cal-QL 的正式论文均与该路线交叉比较，Cal-QL 直接构建于它。

证据入口：理论与跨域实验支持核心机制，多个后续正式论文作为基线或直接扩展，复用与路线价值充分。

具身关联：保守离线 RL 基础方法，TD3+BC、IQL、DT、Trajectory Transformer 和 Cal-QL 的正式论文均与该路线交叉比较，Cal-QL 直接构建于它。

经典保留理由：放宽年限：CQL 是后续多条机器人离线学习路线持续使用的保守价值学习基础与对照，适合先解释分布偏移，再读新策略。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/cql/README.md) · [NeurIPS集锦](../venues/NeurIPS/README.md) · [地图方向](../paper-map/README.md#track-reinforcement-learning) · [首页](../README.md)

元数据核对：2026-10-10。
