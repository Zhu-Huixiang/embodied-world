# Offline Reinforcement Learning as One Big Sequence Modeling Problem

**Trajectory Transformer** · NeurIPS 2021 · 本版排名 73 · 综合分 **83.5 / 100**

[解读导读](../../../library/trajectory-transformer.md) · [世界模型与模型强化学习](../../../paper-map/README.md#track-world-model) · [NeurIPS集锦](../../../venues/NeurIPS/README.md)

[原文](https://proceedings.neurips.cc/paper_files/paper/2021/hash/099fe6b0b444c23836c4a5d07346082b-Abstract.html) · [PDF](https://papers.neurips.cc/paper_files/paper/2021/file/099fe6b0b444c23836c4a5d07346082b-Paper.pdf) · [阅读卡片](../../../library/trajectory-transformer.md)

论文出处：[Michael Janner · UC Berkeley](../../origins/papers/trajectory-transformer.md)

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
| 公开与评审 | 95.0 | 30% |
| 创新性 | 91 | 20% |
| 实验与证据 | 87 | 20% |
| 学术影响 | 46.7 | 10% |
| 近期关注 | 20.3 | 5% |
| 复用价值 | 88 | 8% |
| 阅读价值 | 95 | 7% |

刊会依据：[NeurIPS 2021](../../../venues/NeurIPS/README.md)，正式出处见[出版/原文记录](https://proceedings.neurips.cc/paper_files/paper/2021/hash/099fe6b0b444c23836c4a5d07346082b-Abstract.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：Offline Reinforcement Learning as One Big Sequence Modeling Problem。累计被引 **41**，2025–2026 被引 **7**；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W3213789840) · [文献计量条目](https://openalex.org/W3213789840)

### 影响与关注的计算依据

- **学术影响 46.7**：身份匹配的累计引用C=41，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W3213789840)
- **近期关注 20.3**：近期已定位引用R=7；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W3213789840)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/JannerM/trajectory-transformer) | GitHub Star 537；GitHub Watch订阅 5；GitHub Fork 73 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2106.02039) | HF 论文累计点赞 2 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
