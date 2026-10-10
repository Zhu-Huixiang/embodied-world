# Humanoid Loco-Manipulation With Discrete VLA Model

**Holo-M** · arXiv 2026 · 本版排名 111 · 综合分 **62.3 / 100**

[完整解读](../../../articles/holo-m-2609.35709/README.md) · [视觉语言动作模型 VLA](../../../paper-map/README.md#track-vla) · [arXiv集锦](../../../arxiv/README.md#paper-holo-m)

[原文](https://arxiv.org/abs/2609.35709v1) · [PDF](https://arxiv.org/pdf/2609.35709v1) · [阅读卡片](../../../library/holo-m.md)

论文出处：[Wenxin Shao / Siqi Chai 等3位 · Horizon Robotics GAIL / Horizon Robotics (China)](../../origins/papers/holo-m.md)

[完整中文解读与全篇架构图](../../../articles/holo-m-2609.35709/README.md)

## 机制简析

DCT低频系数与四级残差码固定组长；缺失组监督连接人类/机器人数据，分组恢复接上重叠控制。

带着这个问题读：固定长度动作词表怎样同时连接跨来源数据和控制时钟？

初读判断：固定组长、跨来源有效损失与并行恢复的组合清楚；SIMPLE总分、难格子、消融和两项实机均已逐项读过；实现复用仍需后续跟进。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 60 | 30% |
| 创新性 | 86 | 20% |
| 实验与证据 | 78 | 20% |
| 学术影响 | 0.0 | 10% |
| 近期关注 | 0.0 | 5% |
| 复用价值 | 65 | 8% |
| 阅读价值 | 90 | 7% |

公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；当前阶段为预印本公开。


编辑深度：全文精读；评分记录：2026-10-10。

计量来源：Semantic Scholar；原研究arXiv ID索引记录（版本合并）；匹配题目：Humanoid Loco-Manipulation With Discrete VLA Model。累计被引 **0**，2025–2026 被引 **0**；快照：2026-10-10。

[指标记录](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2609.35709) · [文献计量条目](https://www.semanticscholar.org/paper/8c67b61731a4e5dc87b2b914cfefcf55572c9ebb)

### 影响与关注的计算依据

- **学术影响 0.0**：身份匹配的累计引用C=0，对数压缩上限3000。 [依据1](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2609.35709)
- **近期关注 0.0**：近期已定位引用R=0；数量与每月引用速度各占一半，有效观察期3个月。 [依据1](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2609.35709)

零分表示本次快照已定位的信号处在量表起点；创新和实验两轴分别评价方法。

[其他计量来源快照](../../metrics.json)分别保留，不相加；本版按登记的身份匹配顺序选源。

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
