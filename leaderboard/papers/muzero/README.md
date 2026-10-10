# Mastering Atari, Go, chess and shogi by planning with a learned model

**MuZero** · Nature 2020 · 本版排名 7 · 综合分 **95.1 / 100**

[解读导读](../../../library/muzero.md) · [世界模型与模型强化学习](../../../paper-map/README.md#track-world-model) · [Nature集锦](../../../venues/Nature/README.md)

[原文](https://www.nature.com/articles/s41586-020-03051-4) · [PDF](https://arxiv.org/pdf/1911.08265) · [阅读卡片](../../../library/muzero.md)

## 机制简析

表示网络从观测历史得到潜状态，动力学网络在动作条件下预测下一潜状态和奖励，预测网络给出策略先验和值。MCTS 在这些潜状态里展开候选动作，搜索产生的策略和值再监督网络。Nature 论文比较棋类与 Atari；这里关注的是规划表征，而不是实机机器人结论。

带着这个问题读：用于规划的世界模型，为什么可以只预测奖励、价值和策略，而不重建下一帧？

初读判断：Nature 正式论文、跨棋类和 Atari 的完整实验、公开伪代码；EfficientZero 的直接继承为路线影响提供可核实依据。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 96.8 | 30% |
| 创新性 | 98 | 20% |
| 实验与证据 | 94 | 20% |
| 学术影响 | 88.6 | 10% |
| 近期关注 | 95.9 | 5% |
| 复用价值 | 90 | 8% |
| 阅读价值 | 97 | 7% |

刊会依据：[Nature 2020](../../../venues/Nature/README.md)，正式出处见[出版/原文记录](https://www.nature.com/articles/s41586-020-03051-4)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：正式刊会版本；OpenAlex题目：Mastering Atari, Go, chess and shogi by planning with a learned model。累计被引 1204，2025–2026 被引 388；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W2989847975) · [文献计量条目](https://openalex.org/W2989847975)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
