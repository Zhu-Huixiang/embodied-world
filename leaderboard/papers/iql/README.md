# Offline Reinforcement Learning with Implicit Q-Learning

**IQL** · ICLR 2022 · 本版排名 42 · 综合分 **86.8 / 100**

[解读导读](../../../library/iql.md) · [强化学习与离线决策](../../../paper-map/README.md#track-reinforcement-learning) · [ICLR集锦](../../../venues/ICLR/README.md)

[原文](https://iclr.cc/virtual/2022/poster/5941) · [PDF](https://arxiv.org/pdf/2110.06169) · [阅读卡片](../../../library/iql.md)

论文出处：[**Ilya Kostrikov**](../../origins/papers/iql.md)<br>[加州大学伯克利分校](../../origins/papers/iql.md)

## 机制简析

IQL 在数据动作的 Q 值上做非对称 expectile 回归，拟合偏向较好动作的状态值 V。Q 用奖励加下一状态 V 做 Bellman 更新，策略再按优势加权回归数据中的动作。这个过程把值学习与策略提取拆开，实验用 D4RL 与在线微调检查拼接和改善能力。

带着这个问题读：从未评价数据外动作，IQL 为什么还能拼接次优轨迹并改善策略？

初读判断：算法简洁、公开实现，多域离线基准及微调实验；后续正式论文把它作为比较对象与 Q 引导组件，复用证据明确。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 92 | 20% |
| 实验与证据 | 88 | 20% |
| 学术影响 | 61.0 | 10% |
| 近期关注 | 38.3 | 5% |
| 复用价值 | 96 | 8% |
| 阅读价值 | 95 | 7% |

刊会依据：[ICLR 2022](../../../venues/ICLR/README.md)，正式出处见[出版/原文记录](https://iclr.cc/virtual/2022/poster/5941)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：Offline Reinforcement Learning with Implicit Q-Learning。累计被引 **131**，2025–2026 被引 **29**；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W3205794883) · [文献计量条目](https://openalex.org/W3205794883)

### 影响与关注的计算依据

- **学术影响 61.0**：身份匹配的累计引用C=131，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W3205794883)
- **近期关注 38.3**：近期已定位引用R=29；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W3205794883)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/ikostrikov/implicit_q_learning) | GitHub Star 338；GitHub Watch订阅 3；GitHub Fork 49 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2110.06169) | HF 论文累计点赞 0 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
