# Offline Reinforcement Learning as One Big Sequence Modeling Problem

**Trajectory Transformer** · NeurIPS 2021 · 本版排名 66 · 综合分 **84.1 / 100**

[解读导读](../../../library/trajectory-transformer.md) · [世界模型与模型强化学习](../../../paper-map/README.md#track-world-model) · [NeurIPS集锦](../../../venues/NeurIPS/README.md)

[原文](https://proceedings.neurips.cc/paper_files/paper/2021/hash/099fe6b0b444c23836c4a5d07346082b-Abstract.html) · [PDF](https://papers.neurips.cc/paper_files/paper/2021/file/099fe6b0b444c23836c4a5d07346082b-Paper.pdf) · [阅读卡片](../../../library/trajectory-transformer.md)

## 机制简析

把状态和动作各维离散化，与奖励串成 token，Transformer 联合学习整段轨迹的概率。规划时用 beam search 保留高回报候选轨迹，执行第一步后重新搜索；稀疏长时序任务还可以接 IQL 的 Q 值做搜索启发。原文同时检查长预测误差、模仿、目标到达与离线 RL。

带着这个问题读：状态、动作和奖励一起变成 token 后，beam search 为什么可以用来规划？

初读判断：完整模型/规划链路与多个控制设定，直接比较 DT、CQL 和 IQL；后续 Diffuser 改变生成方式但延续整轨迹规划问题。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 91 | 20% |
| 实验与证据 | 87 | 20% |
| 学术影响 | 46.7 | 10% |
| 近期关注 | 33.4 | 5% |
| 复用价值 | 88 | 8% |
| 阅读价值 | 95 | 7% |

刊会依据：[NeurIPS 2021](../../../venues/NeurIPS/README.md)，正式出处见[出版/原文记录](https://proceedings.neurips.cc/paper_files/paper/2021/hash/099fe6b0b444c23836c4a5d07346082b-Abstract.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：Offline Reinforcement Learning as One Big Sequence Modeling Problem。累计被引 41，2025–2026 被引 7；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W3213789840) · [文献计量条目](https://openalex.org/W3213789840)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
