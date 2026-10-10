# PLaW-VLA: Predictive Latent World Modeling for Vision-Language-Action Policies

**PLaW-VLA** · arXiv 2026 · 本版排名 115 · 综合分 **61.7 / 100**

[解读导读](../../../library/plaw-vla.md) · [视频动作模型与视觉推理](../../../paper-map/README.md#track-video-action) · [arXiv集锦](../../../arxiv/README.md#paper-plaw-vla)

[原文](https://arxiv.org/abs/2610.12285v1) · [PDF](https://arxiv.org/pdf/2610.12285v1) · [阅读卡片](../../../library/plaw-vla.md)

论文出处：[Yu Liu / Hetian Guo · Jilin University / Astribot 等5个出处](../../origins/papers/plaw-vla.md)

## 机制简析

预测面向任务的未来潜表示，再用结构化因果注意力让动作生成读取历史、任务和未来状态，减少无关像素重建。

带着这个问题读：怎样证明预测的未来表征真的帮助长程动作？

初读判断：有响应式策略与重建表示对照线索；初读优先看长程任务、未来预测和注意力结构消融。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 60 | 30% |
| 创新性 | 84 | 20% |
| 实验与证据 | 75 | 20% |
| 学术影响 | 0 | 10% |
| 近期关注 | 11.9 | 5% |
| 复用价值 | 63 | 8% |
| 阅读价值 | 89 | 7% |

公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；当前阶段为预印本公开。


编辑深度：选题初读；评分记录：2026-10-10。

计量来源：Semantic Scholar；原研究arXiv ID索引记录（版本合并）；匹配题目：PLaW-VLA: Predictive Latent World Modeling for Vision-Language-Action Policies。累计被引 **0**，2025–2026 被引 **0**；快照：2026-10-10。

[指标记录](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2610.12285) · [文献计量条目](https://www.semanticscholar.org/paper/cf78191c38ce27bbe2993af31890a205c0f14a85)

### 影响与关注的计算依据

- **学术影响 0**：本次已定位的独立采用/讨论证据处于量表起点；引用与专属仓库关注另算，取最高已核信号。 [依据1](https://arxiv.org/abs/2610.12285v1) · [依据2](https://github.com/Zhu-Huixiang/embodied-world/blob/main/leaderboard/selection-2026-10-10.md)
- **近期关注 11.9**：近期窗口内创建的专属论文仓库，快照star=2；按10000上限对数压缩。 [依据1](https://api.github.com/repos/RainyRobo/PLaW-VLA) · [依据2](https://raw.githubusercontent.com/RainyRobo/PLaW-VLA/main/README.md)

零分表示本次快照已定位的信号处在量表起点；创新和实验两轴分别评价方法。

[其他计量来源快照](../../metrics.json)分别保留，不相加；本版按登记的身份匹配顺序选源。

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/RainyRobo/PLaW-VLA) | GitHub Star 2；GitHub Watch订阅 0；GitHub Fork 2 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
