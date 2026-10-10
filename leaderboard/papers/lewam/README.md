# LeWAM: A JEPA World Action Model with Diffusion-Steering-Based MPC

**LeWAM** · arXiv 2026 · 本版排名 110 · 综合分 **63.1 / 100**

[解读导读](../../../library/lewam.md) · [世界动作模型](../../../paper-map/README.md#track-world-action-model) · [arXiv集锦](../../../arxiv/README.md#paper-lewam)

[原文](https://arxiv.org/abs/2610.12407v1) · [PDF](https://arxiv.org/pdf/2610.12407v1) · [阅读卡片](../../../library/lewam.md)

论文出处：[**Shashank Hegde**](../../origins/papers/lewam.md)<br>[英伟达](../../origins/papers/lewam.md)

## 机制简析

在不重建图像的 JEPA 表征上联合学前向、后向、逆动力学和策略；MPC 在策略噪声空间采样，降低规划钻动力学模型空子的机会。

带着这个问题读：联合表征怎样支持预测、动作生成和闭环规划？

初读判断：潜世界动作模型与噪声空间规划贴合本仓路线；有同编码器/规模对照线索，优先追规划消融。

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
| 实验与证据 | 76 | 20% |
| 学术影响 | 0 | 10% |
| 近期关注 | 0 | 5% |
| 复用价值 | 64 | 8% |
| 阅读价值 | 94 | 7% |

公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；当前阶段为预印本公开。


编辑深度：选题初读；评分记录：2026-10-10。

计量来源：Semantic Scholar；原研究arXiv ID索引记录（版本合并）；匹配题目：LeWAM: A JEPA World Action Model with Diffusion-Steering-Based MPC。累计被引 **0**，2025–2026 被引 **0**；快照：2026-10-10。

[指标记录](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2610.12407) · [文献计量条目](https://www.semanticscholar.org/paper/d75db25eda3ce772ceeb52bdd25fb057699c3972)

### 影响与关注的计算依据

- **学术影响 0**：本次已定位的独立采用/讨论证据处于量表起点；引用与专属仓库关注另算，取最高已核信号。 [依据1](https://arxiv.org/abs/2610.12407v1) · [依据2](https://github.com/Zhu-Huixiang/embodied-world/blob/main/leaderboard/selection-2026-10-10.md)
- **近期关注 0**：本次已定位的独立采用/讨论证据处于量表起点；引用与专属仓库关注另算，取最高已核信号。 [依据1](https://arxiv.org/abs/2610.12407v1) · [依据2](https://github.com/Zhu-Huixiang/embodied-world/blob/main/leaderboard/selection-2026-10-10.md)

零分表示本次快照已定位的信号处在量表起点；创新和实验两轴分别评价方法。

[其他计量来源快照](../../metrics.json)分别保留，不相加；本版按登记的身份匹配顺序选源。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
