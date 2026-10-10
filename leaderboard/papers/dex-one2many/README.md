# Dex-One2Many: Learning Dexterous Manipulation from a Single Human Demonstration

**Dex-One2Many** · arXiv 2026 · 本版排名 112 · 综合分 **62.2 / 100**

[解读导读](../../../library/dex-one2many.md) · [操作与动作块](../../../paper-map/README.md#track-manipulation) · [arXiv集锦](../../../arxiv/README.md#paper-dex-one2many)

[原文](https://arxiv.org/abs/2610.12470v1) · [PDF](https://arxiv.org/pdf/2610.12470v1) · [阅读卡片](../../../library/dex-one2many.md)

论文出处：[Jusuk Lee · Seoul National University / University of Maryland 等4个出处](../../origins/papers/dex-one2many.md)

## 机制简析

把单视频压成顺序场景关系图，以图约束重置状态、阶段奖励，指导 RL 搜索更广的抓取与物体配置。

带着这个问题读：场景图怎样同时提供探索引导与不锁死姿态的泛化？

初读判断：单视频灵巧操作；摘要给出五项任务、对照与实机转移；优先检查重置采样和奖励消融。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 60 | 30% |
| 创新性 | 88 | 20% |
| 实验与证据 | 76 | 20% |
| 学术影响 | 0 | 10% |
| 近期关注 | 0 | 5% |
| 复用价值 | 65 | 8% |
| 阅读价值 | 89 | 7% |

公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；当前阶段为预印本公开。


编辑深度：选题初读；评分记录：2026-10-10。

计量来源：Semantic Scholar；原研究arXiv ID索引记录（版本合并）；匹配题目：Dex-One2Many: Learning Dexterous Manipulation from a Single Human Demonstration。累计被引 **0**，2025–2026 被引 **0**；快照：2026-10-10。

[指标记录](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2610.12470) · [文献计量条目](https://www.semanticscholar.org/paper/50c9fac4af15c05f80944a9e40dd5f3718aea59a)

### 影响与关注的计算依据

- **学术影响 0**：本次已定位的独立采用/讨论证据处于量表起点；引用与专属仓库关注另算，取最高已核信号。 [依据1](https://arxiv.org/abs/2610.12470v1) · [依据2](https://github.com/Zhu-Huixiang/embodied-world/blob/main/leaderboard/selection-2026-10-10.md)
- **近期关注 0**：本次已定位的独立采用/讨论证据处于量表起点；引用与专属仓库关注另算，取最高已核信号。 [依据1](https://arxiv.org/abs/2610.12470v1) · [依据2](https://github.com/Zhu-Huixiang/embodied-world/blob/main/leaderboard/selection-2026-10-10.md)

零分表示本次快照已定位的信号处在量表起点；创新和实验两轴分别评价方法。

[其他计量来源快照](../../metrics.json)分别保留，不相加；本版按登记的身份匹配顺序选源。

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
