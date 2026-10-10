# Decision Transformer: Reinforcement Learning via Sequence Modeling

**解读导读** · NeurIPS 2021 · [强化学习与离线决策](../paper-map/README.md#track-reinforcement-learning)

研究范围：序列决策基础；离线控制。

[原文入口](https://proceedings.neurips.cc/paper_files/paper/2021/hash/7f489f642a0ddb10272b5c31057f0663-Abstract.html) · [原文 PDF](https://proceedings.neurips.cc/paper_files/paper/2021/file/7f489f642a0ddb10272b5c31057f0663-Paper.pdf)

## 先看它做了什么

把未来目标回报、状态和动作按时间交错成序列，因果 Transformer 用过去上下文预测当前动作。训练直接拟合数据动作；执行后减去已经获得的奖励，再把更新后的目标回报与新状态送回模型。实验用 Atari、Gym 与长时序任务检验这个条件生成式策略。

## 带着什么问题读

**把目标回报放进 token 序列，就能把离线控制改写成条件生成吗？**

## 为什么值得继续读

把决策问题接到 Transformer 的代表性路线；Trajectory Transformer 原文与它比较规划和回报条件化，适合进入动作语言模型的前置阅读。

证据入口：方法提出清晰的新决策表述，正式论文跨离散与连续域，后续 Trajectory Transformer 对其优缺点作直接比较。

具身关联：把决策问题接到 Transformer 的代表性路线；Trajectory Transformer 原文与它比较规划和回报条件化，适合进入动作语言模型的前置阅读。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/decision-transformer/README.md) · [NeurIPS集锦](../venues/NeurIPS/README.md) · [地图方向](../paper-map/README.md#track-reinforcement-learning) · [首页](../README.md)

元数据核对：2026-10-10。
