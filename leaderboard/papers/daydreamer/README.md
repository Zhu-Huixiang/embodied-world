# DayDreamer: World Models for Physical Robot Learning

**DayDreamer** · CoRL 2022 · 本版排名 83 · 综合分 **82.2 / 100**

[解读导读](../../../library/daydreamer.md) · [世界模型与模型强化学习](../../../paper-map/README.md#track-world-model) · [CoRL集锦](../../../venues/CoRL/README.md)

[原文](https://proceedings.mlr.press/v205/wu23c.html) · [PDF](https://proceedings.mlr.press/v205/wu23c/wu23c.pdf) · [阅读卡片](../../../library/daydreamer.md)

论文出处：[**Philipp Wu / Alejandro Escontrela 等3位**](../../origins/papers/daydreamer.md)<br>[加州大学伯克利分校](../../origins/papers/daydreamer.md)

## 机制简析

真实机器人持续把轨迹写入经验回放，学习线程更新潜空间世界模型，再用模型想象的轨迹训练策略和值函数。异步 actor 与 learner 把快速执行和较慢训练拆开，避免每次梯度更新卡住机器人控制。原文用四足、两种机械臂和轮式机器人检查同一算法的在线学习能力。

带着这个问题读：世界模型的想象训练怎样接到真实机器人持续在线交互上？

初读判断：有多平台实机闭环与明确训练时间、学习曲线和基线；公开基础设施，使世界模型精讲能落到真实采样链路。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 90.0 | 30% |
| 创新性 | 87 | 20% |
| 实验与证据 | 91 | 20% |
| 学术影响 | 48.1 | 10% |
| 近期关注 | 20.3 | 5% |
| 复用价值 | 89 | 8% |
| 阅读价值 | 95 | 7% |

刊会依据：[CoRL 2022](../../../venues/CoRL/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v205/wu23c.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：DayDreamer: World Models for Physical Robot Learning。累计被引 **46**，2025–2026 被引 **7**；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W4283721947) · [文献计量条目](https://openalex.org/W4283721947)

### 影响与关注的计算依据

- **学术影响 48.1**：身份匹配的累计引用C=46，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4283721947)
- **近期关注 20.3**：近期已定位引用R=7；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W4283721947)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/danijar/daydreamer) | GitHub Star 465；GitHub Watch订阅 9；GitHub Fork 46 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2206.14176) | HF 论文累计点赞 0 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
