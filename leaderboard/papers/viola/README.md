# VioLA: Learning Generalist Humanoid Control Policies from Human Data

**VIOLA** · arXiv 2026 · 本版排名 109 · 综合分 **63.8 / 100**

[解读导读](../../../library/viola.md) · [视觉语言动作模型 VLA](../../../paper-map/README.md#track-vla) · [arXiv集锦](../../../arxiv/README.md#paper-viola)

[原文](https://arxiv.org/abs/2610.12435v1) · [PDF](https://arxiv.org/pdf/2610.12435v1) · [阅读卡片](../../../library/viola.md)

论文出处：[**Mert Albaba**](../../origins/papers/viola.md)<br>[Vesoma / 苏黎世联邦理工学院 · 另3个机构](../../origins/papers/viola.md)

## 机制简析

VLA 预测身体与手部运动 latent，预训练控制器负责执行；运动编码器把人类示范映射到同一空间，扩大可监督动作池。

带着这个问题读：人类动作怎样先对齐控制器，再教会人形 VLA？

初读判断：跨数据监督和动作空间转换直接对上 Holo-M；初读关注零样本协议、控制器预训练与总数据规模。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 60 | 30% |
| 创新性 | 91 | 20% |
| 实验与证据 | 79 | 20% |
| 学术影响 | 0 | 10% |
| 近期关注 | 0 | 5% |
| 复用价值 | 65 | 8% |
| 阅读价值 | 94 | 7% |

公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；当前阶段为预印本公开。


编辑深度：选题初读；评分记录：2026-10-10。

计量来源：Semantic Scholar；原研究arXiv ID索引记录（版本合并）；匹配题目：VioLA: Learning Generalist Humanoid Control Policies from Human Data。累计被引 **0**，2025–2026 被引 **0**；快照：2026-10-10。

[指标记录](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2610.12435) · [文献计量条目](https://www.semanticscholar.org/paper/ce1875ec86d2e7940f6b0035d6dc01b54472a6ef)

### 影响与关注的计算依据

- **学术影响 0**：本次已定位的独立采用/讨论证据处于量表起点；引用与专属仓库关注另算，取最高已核信号。 [依据1](https://arxiv.org/abs/2610.12435v1) · [依据2](https://github.com/Zhu-Huixiang/embodied-world/blob/main/leaderboard/selection-2026-10-10.md)
- **近期关注 0**：本次已定位的独立采用/讨论证据处于量表起点；引用与专属仓库关注另算，取最高已核信号。 [依据1](https://arxiv.org/abs/2610.12435v1) · [依据2](https://github.com/Zhu-Huixiang/embodied-world/blob/main/leaderboard/selection-2026-10-10.md)

零分表示本次快照已定位的信号处在量表起点；创新和实验两轴分别评价方法。

[其他计量来源快照](../../metrics.json)分别保留，不相加；本版按登记的身份匹配顺序选源。

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
