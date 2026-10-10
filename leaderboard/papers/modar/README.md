# Modality-Autoregressive World-Action Models

**ModAR** · arXiv 2026 · 本版排名 107 · 综合分 **69.6 / 100**

[解读导读](../../../library/modar.md) · [世界动作模型](../../../paper-map/README.md#track-world-action-model) · [arXiv集锦](../../../arxiv/README.md#paper-modar)

[原文](https://arxiv.org/abs/2609.17524v1) · [PDF](https://arxiv.org/pdf/2609.17524v1) · [阅读卡片](../../../library/modar.md)

论文出处：[**Adam Hung**](../../origins/papers/modar.md)<br>[卡内基梅隆大学](../../origins/papers/modar.md)

## 机制简析

共享DiT把当前DINO/深度/RGB和配置/任务条件融合，按点轨迹→DINO→深度→RGB块自回归去噪，动作最后生成；上下文加噪避免前一模态误差层层放大。实机去掉收益最小的未来RGB。

带着这个问题读：为什么先预测点轨迹、语义与几何，再给动作，可能比视频动作一起去噪更有效？

初读判断：新意在模态顺序和可控比较，独立IDM、匹配40采样步、模态/顺序/上下文噪声消融支撑机制。实机3任务90rollouts每模型，总体外推有限；仅比较一个反序，按best checkpoint在同批held-out条件报数，不能当跨域无偏评估。代码可复用情况未完整核，reuse不按想象给高分。

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
| 实验与证据 | 85 | 20% |
| 学术影响 | 8.7 | 10% |
| 近期关注 | 76.5 | 5% |
| 复用价值 | 72 | 8% |
| 阅读价值 | 94 | 7% |

公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；当前阶段为预印本公开。


编辑深度：选题初读（方法、实验与消融）；评分记录：2026-10-10。

计量来源：Semantic Scholar；原研究arXiv ID索引记录（版本合并）；匹配题目：Modality-Autoregressive World-Action Models。累计被引 **1**，2025–2026 被引 **1**；快照：2026-10-10。

[指标记录](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2609.17524) · [文献计量条目](https://www.semanticscholar.org/paper/3395cd60d241d839df377d379639ca85ca7c1d9f)

### 影响与关注的计算依据

- **学术影响 8.7**：身份匹配的累计引用C=1，对数压缩上限3000。 [依据1](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2609.17524)
- **近期关注 76.5**：x 的论文专属入口：Views=38777；按1000000上限对数压缩。 [依据1](https://x.com/Adamjhung/status/2100268484592869557)

[其他计量来源快照](../../metrics.json)分别保留，不相加；本版按登记的身份匹配顺序选源。

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/adamhung60/ModAR-code) | GitHub Star 14；GitHub Watch订阅 0；GitHub Fork 2 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2609.17524) | HF 论文累计点赞 11 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |
| [x](https://x.com/Adamjhung/status/2100268484592869557) | Views 38777；Likes 410；Reposts 61；Replies 13；Quotes 5；Bookmarks 352 | 单篇论文入口；截至2026-10-10的累计快照 | 2026-10-10T15:21:08.510932+08:00 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
