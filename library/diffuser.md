# Planning with Diffusion for Flexible Behavior Synthesis

**解读导读** · ICML 2022 · [世界动作模型](../paper-map/README.md#track-world-action-model)

研究范围：扩散轨迹规划基础；模拟控制。

[原文入口](https://proceedings.mlr.press/v162/janner22a.html) · [原文 PDF](https://proceedings.mlr.press/v162/janner22a/janner22a.pdf) · [作者项目 / 代码入口](https://diffusion-planning.github.io/) · [作者与团队](../leaderboard/origins/papers/diffuser.md)

## 先看它做了什么

Diffuser 学习整段状态—动作轨迹的去噪过程，反复修正所有规划时刻，而不是单步滚动一个动力学模型。奖励梯度可以引导去噪，固定起点或终点则像图像补全那样锁住轨迹部分。论文在长时序与灵活测试条件下比较规划效果，并区分扩散步和环境时间步。

## 带着什么问题读

**轨迹一起去噪，如何同时承担环境建模、长时序规划与测试时加约束？**

## 为什么值得继续读

扩散生成接到控制规划的基础论文，区别于只生成一步动作，适合解释后续扩散策略和世界动作模型的来路。

证据入口：提出可组合的生成式规划框架，有长时序控制及条件变化实验，正式 ICML 论文和官方项目可复核。

具身关联：扩散生成接到控制规划的基础论文，区别于只生成一步动作，适合解释后续扩散策略和世界动作模型的来路。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/diffuser/README.md) · [ICML集锦](../venues/ICML/README.md) · [地图方向](../paper-map/README.md#track-world-action-model) · [首页](../README.md)

元数据核对：2026-10-10。
