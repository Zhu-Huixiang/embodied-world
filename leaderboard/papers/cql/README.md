# Conservative Q-Learning for Offline Reinforcement Learning

**CQL** · NeurIPS 2020 · 本版排名 20 · 综合分 **91.1 / 100**

[解读导读](../../../library/cql.md) · [强化学习与离线决策](../../../paper-map/README.md#track-reinforcement-learning) · [NeurIPS集锦](../../../venues/NeurIPS/README.md)

[原文](https://proceedings.neurips.cc/paper_files/paper/2020/hash/0d2b2061826a5df3221116a5085a6052-Abstract.html) · [PDF](https://papers.nips.cc/paper_files/paper/2020/file/0d2b2061826a5df3221116a5085a6052-Paper.pdf) · [阅读卡片](../../../library/cql.md)

## 机制简析

CQL 在 Bellman 误差外增加正则：压低策略或广泛采样动作的 Q 值，相对抬高数据动作的 Q 值。得到的保守值函数用于策略改进，从而减少数据外动作被过高估计的风险。原文同时给出值下界分析、离散与连续控制实验及复杂数据分布比较。

带着这个问题读：离线数据没有覆盖的动作，怎样避免被 Q 函数凭空吹成好动作？

初读判断：理论与跨域实验支持核心机制，多个后续正式论文作为基线或直接扩展，复用与路线价值充分。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 95 | 20% |
| 实验与证据 | 89 | 20% |
| 学术影响 | 78.9 | 10% |
| 近期关注 | 70.5 | 5% |
| 复用价值 | 97 | 8% |
| 阅读价值 | 95 | 7% |

刊会依据：[NeurIPS 2020](../../../venues/NeurIPS/README.md)，正式出处见[出版/原文记录](https://proceedings.neurips.cc/paper_files/paper/2020/hash/0d2b2061826a5df3221116a5085a6052-Abstract.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：Conservative Q-Learning for Offline Reinforcement Learning。累计被引 554，2025–2026 被引 79；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W3033324992) · [文献计量条目](https://openalex.org/W3033324992)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
