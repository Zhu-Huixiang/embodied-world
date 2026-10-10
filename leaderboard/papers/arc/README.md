# ARC: A Reasoning Recipe for Robot Foundation Models

**ARC** · arXiv 2026 · 本版排名 113 · 综合分 **62.2 / 100**

[解读导读](../../../library/arc.md) · [视觉语言动作模型 VLA](../../../paper-map/README.md#track-vla) · [arXiv集锦](../../../arxiv/README.md#paper-arc)

[原文](https://arxiv.org/abs/2610.12386v1) · [PDF](https://arxiv.org/pdf/2610.12386v1) · [阅读卡片](../../../library/arc.md)

论文出处：[Gokul Puthumanaillam · University of Illinois Urbana-Champaign / Stanford University 等5个出处](../../origins/papers/arc.md)

## 机制简析

给现有示范自动添“下一动作为什么合适、会造成什么”的推理轨迹，再按 VLA/WAM 架构适配推理与动作输出。

带着这个问题读：推理文字怎样成为动作条件，而不是另一段好看的解说？

初读判断：推理与控制的明确接口；初读关注自动标注质量、不同基础策略的匹配训练和零样本条件。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 60 | 30% |
| 创新性 | 87 | 20% |
| 实验与证据 | 76 | 20% |
| 学术影响 | 0 | 10% |
| 近期关注 | 0 | 5% |
| 复用价值 | 65 | 8% |
| 阅读价值 | 91 | 7% |

公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；当前阶段为预印本公开。


编辑深度：选题初读；评分记录：2026-10-10。

计量来源：Semantic Scholar；原研究arXiv ID索引记录（版本合并）；匹配题目：ARC: A Reasoning Recipe for Robot Foundation Models。累计被引 **0**，2025–2026 被引 **0**；快照：2026-10-10。

[指标记录](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2610.12386) · [文献计量条目](https://www.semanticscholar.org/paper/ac921f84b421bac30c0d27bba5b79d7215062e8d)

### 影响与关注的计算依据

- **学术影响 0**：本次已定位的独立采用/讨论证据处于量表起点；引用与专属仓库关注另算，取最高已核信号。 [依据1](https://arxiv.org/abs/2610.12386v1) · [依据2](https://github.com/Zhu-Huixiang/embodied-world/blob/main/leaderboard/selection-2026-10-10.md)
- **近期关注 0**：本次已定位的独立采用/讨论证据处于量表起点；引用与专属仓库关注另算，取最高已核信号。 [依据1](https://arxiv.org/abs/2610.12386v1) · [依据2](https://github.com/Zhu-Huixiang/embodied-world/blob/main/leaderboard/selection-2026-10-10.md)

零分表示本次快照已定位的信号处在量表起点；创新和实验两轴分别评价方法。

[其他计量来源快照](../../metrics.json)分别保留，不相加；本版按登记的身份匹配顺序选源。

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
