# World Action Models are Zero-shot Policies

**DreamZero** · arXiv 2026 · 本版排名 98 · 综合分 **80.1 / 100**

[解读导读](../../../library/dreamzero.md) · [世界动作模型](../../../paper-map/README.md#track-world-action-model) · [arXiv集锦](../../../arxiv/README.md#paper-dreamzero)

[原文](https://arxiv.org/abs/2602.15922) · [PDF](https://arxiv.org/pdf/2602.15922) · [阅读卡片](../../../library/dreamzero.md)

论文出处：[Seonghyeon Ye · NVIDIA GEAR / NVIDIA](../../origins/papers/dreamzero.md)

## 机制简析

联合建模未来视频与动作，将大规模视觉动态先验用于未见任务的闭环策略。

带着这个问题读：视频与动作共同预测，怎样支持未见任务中的控制？

初读判断：WAM零样本任务分歧清楚；初读仍要按数据、未见任务划分和控制时钟拆证据。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 65 | 30% |
| 创新性 | 93 | 20% |
| 实验与证据 | 82 | 20% |
| 学术影响 | 77.0 | 10% |
| 近期关注 | 99.5 | 5% |
| 复用价值 | 79 | 8% |
| 阅读价值 | 95 | 7% |

公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；当前阶段为预印本公开。；独立公开技术检验阶段65，取较高阶段。


编辑深度：选题初读；评分记录：2026-10-10。

计量来源：Semantic Scholar；原研究arXiv ID索引记录（版本合并）；匹配题目：World Action Models are Zero-shot Policies。累计被引 **474**，2025–2026 被引 **至少 469**；快照：2026-10-10。

[指标记录](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2602.15922) · [文献计量条目](https://www.semanticscholar.org/paper/badf8adcf2b6a6780a308881de75f148a4cacea0)

### 影响与关注的计算依据

- **学术影响 77.0**：身份匹配的累计引用C=474，对数压缩上限3000。 [依据1](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2602.15922)
- **近期关注 99.5**：近期已定位引用R=469；数量与每月引用速度各占一半，有效观察期7.7207个月。 [依据1](https://api.semanticscholar.org/graph/v1/paper/badf8adcf2b6a6780a308881de75f148a4cacea0/citations)

[其他计量来源快照](../../metrics.json)分别保留，不相加；本版按登记的身份匹配顺序选源。

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/dreamzero0/dreamzero) | GitHub Star 2699；GitHub Watch订阅 17；GitHub Fork 243 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/GEAR-Dreams/DreamZero-DROID) | HF 最近30天下载 1566；HF 仓库累计点赞 37 | 单篇论文的作者发布资产；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2602.15922) | HF 论文累计点赞 20 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |
| [linkedin](https://www.linkedin.com/posts/drjimfan_introducing-dreamzero-we-trained-a-robot-activity-7425206585091579905-pHMe) | Reactions 1547；Comments 62 | 单篇论文入口；截至2026-10-10的累计快照 | 2026-10-10T15:21:08.510785+08:00 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
