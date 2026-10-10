# EgoScale: Scaling Dexterous Manipulation with Diverse Egocentric Human Data

**EgoScale** · arXiv 2026 · 本版排名 105 · 综合分 **75.6 / 100**

[解读导读](../../../library/egoscale.md) · [操作与动作块](../../../paper-map/README.md#track-manipulation) · [arXiv集锦](../../../arxiv/README.md#paper-egoscale)

[原文](https://arxiv.org/abs/2602.16710) · [PDF](https://arxiv.org/pdf/2602.16710v1) · [阅读卡片](../../../library/egoscale.md)

论文出处：[**Ruijie Zheng / Dantong Niu 等3位**](../../origins/papers/egoscale.md)<br>[英伟达 GEAR 研究团队 / 英伟达 · 另2个机构](../../origins/papers/egoscale.md)

## 机制简析

从第一视角human videos提取相对SE(3)腕部轨迹与重定向22DoF手关节，pretrain flow-based VLA；少量paired human/robot play midtraining对齐视觉和motor接口，再任务posttrain。统一腕部action、embodiment-specific hand/state adapters迁移至G1 7DoF手，下肢独立Homie。

带着这个问题读：人类视频怎样变成机器人可学的手腕和手指动作，为什么大量预训练之后还要一小段人机对齐数据？

初读判断：动作级human supervision、规模规律与aligned transfer组合有价值。五项实机、1k–20k小时五档规模、表示/两阶段消融和跨手型证据较丰富，但有限seed/trials、专有大数据与未全面开源、one-shot附加human supervision限制证据和复用分；R²是五个规模点内fit，不预测全域能力。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 60 | 30% |
| 创新性 | 89 | 20% |
| 实验与证据 | 84 | 20% |
| 学术影响 | 60.3 | 10% |
| 近期关注 | 86.4 | 5% |
| 复用价值 | 78 | 8% |
| 阅读价值 | 92 | 7% |

公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；当前阶段为预印本公开。


编辑深度：原文机制与实验初读；评分记录：2026-10-10。

计量来源：Semantic Scholar；原研究arXiv ID索引记录（版本合并）；匹配题目：EgoScale: Scaling Dexterous Manipulation with Diverse Egocentric Human Data。累计被引 **124**，2025–2026 被引 **至少 123**；快照：2026-10-10。

[指标记录](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2602.16710) · [文献计量条目](https://www.semanticscholar.org/paper/a51ce1a04c9da80f399d81fd5cf4b3e4fd2285e7)

### 影响与关注的计算依据

- **学术影响 60.3**：身份匹配的累计引用C=124，对数压缩上限3000。 [依据1](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2602.16710)
- **近期关注 86.4**：linkedin 的论文专属入口：Reactions=2863；按10000上限对数压缩。 [依据1](https://www.linkedin.com/posts/drjimfan_we-trained-a-humanoid-with-22-dof-dexterous-activity-7432471307633713152-q2Xn)

[其他计量来源快照](../../metrics.json)分别保留，不相加；本版按登记的身份匹配顺序选源。

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [huggingface](https://huggingface.co/papers/2602.16710) | HF 论文累计点赞 1 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |
| [linkedin](https://www.linkedin.com/posts/drjimfan_we-trained-a-humanoid-with-22-dof-dexterous-activity-7432471307633713152-q2Xn) | Reactions 2863；Comments 129 | 单篇论文入口；截至2026-10-10的累计快照 | 2026-10-10T15:21:08.510623+08:00 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
