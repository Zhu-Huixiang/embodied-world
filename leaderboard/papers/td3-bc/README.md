# A Minimalist Approach to Offline Reinforcement Learning

**TD3+BC** · NeurIPS 2021 · 本版排名 59 · 综合分 **84.8 / 100**

[解读导读](../../../library/td3-bc.md) · [强化学习与离线决策](../../../paper-map/README.md#track-reinforcement-learning) · [NeurIPS集锦](../../../venues/NeurIPS/README.md)

[原文](https://proceedings.neurips.cc/paper/2021/hash/a8166da05c5a094f7dc03724b41886e5-Abstract.html) · [PDF](https://proceedings.neurips.cc/paper/2021/file/a8166da05c5a094f7dc03724b41886e5-Paper.pdf) · [阅读卡片](../../../library/td3-bc.md)

论文出处：[**Scott Fujimoto**](../../origins/papers/td3-bc.md)<br>[魁北克人工智能研究所（Mila） / 麦吉尔大学 · 另1个机构](../../origins/papers/td3-bc.md)

## 机制简析

TD3+BC 保留 TD3 的双 Q 与 actor-critic 框架，在策略目标里同时提高 Q 值并拉近策略动作和数据动作。状态标准化稳定输入尺度，Q 值归一化的系数平衡价值追求与行为克隆。原文在 D4RL 连续控制中重跑部分基线，并报告性能与计算成本。

带着这个问题读：只在 TD3 策略损失里加一个模仿项，为什么能成为可靠的离线 RL 基线？

初读判断：贡献集中且容易实现；固定数据基准、基线重跑和性能/成本比较支持其基线价值，后续离线到在线研究明确复用。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 82 | 20% |
| 实验与证据 | 87 | 20% |
| 学术影响 | 63.5 | 10% |
| 近期关注 | 40.2 | 5% |
| 复用价值 | 96 | 8% |
| 阅读价值 | 92 | 7% |

刊会依据：[NeurIPS 2021](../../../venues/NeurIPS/README.md)，正式出处见[出版/原文记录](https://proceedings.neurips.cc/paper/2021/hash/a8166da05c5a094f7dc03724b41886e5-Abstract.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：A Minimalist Approach to Offline Reinforcement Learning。累计被引 **160**，2025–2026 被引 **33**；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W3172360140) · [文献计量条目](https://openalex.org/W3172360140)

### 影响与关注的计算依据

- **学术影响 63.5**：身份匹配的累计引用C=160，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W3172360140)
- **近期关注 40.2**：近期已定位引用R=33；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W3172360140)
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
