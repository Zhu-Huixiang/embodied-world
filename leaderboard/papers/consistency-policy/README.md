# Consistency Policy: Accelerated Visuomotor Policies via Consistency Distillation

**Consistency Policy** · RSS 2024 · 本版排名 93 · 综合分 **80.7 / 100**

[解读导读](../../../library/consistency-policy.md) · [操作与动作块](../../../paper-map/README.md#track-manipulation) · [RSS集锦](../../../venues/RSS/README.md)

[原文](https://www.roboticsproceedings.org/rss20/p071.html) · [PDF](https://www.roboticsproceedings.org/rss20/p071.pdf) · [阅读卡片](../../../library/consistency-policy.md)

论文出处：[Aaditya Prasad · Stanford University / Princeton University](../../origins/papers/consistency-policy.md)

## 机制简析

将多步扩散动作策略蒸馏为较少步的一致性策略，以减少推理步骤保留动作分布。

带着这个问题读：蒸馏怎样减少去噪步骤，保留怎样的动作分布？

初读判断：速度/成功率取舍明确；作为控制时钟的对照非常合适。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 81 | 20% |
| 实验与证据 | 80 | 20% |
| 学术影响 | 49.8 | 10% |
| 近期关注 | 48.0 | 5% |
| 复用价值 | 82 | 8% |
| 阅读价值 | 86 | 7% |

刊会依据：[RSS 2024](../../../venues/RSS/README.md)，正式出处见[出版/原文记录](https://www.roboticsproceedings.org/rss20/p071.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：选题初读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：Consistency Policy: Accelerated Visuomotor Policies via Consistency Distillation。累计被引 **53**，2025–2026 被引 **53**；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W4402354007) · [文献计量条目](https://openalex.org/W4402354007)

### 影响与关注的计算依据

- **学术影响 49.8**：身份匹配的累计引用C=53，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4402354007)
- **近期关注 48.0**：近期已定位引用R=53；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W4402354007)
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
