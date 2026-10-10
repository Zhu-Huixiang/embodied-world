# Mastering Atari with Discrete World Models

**DreamerV2** · ICLR 2021 · 本版排名 81 · 综合分 **82.4 / 100**

[解读导读](../../../library/dreamerv2.md) · [世界模型与模型强化学习](../../../paper-map/README.md#track-world-model) · [ICLR集锦](../../../venues/ICLR/README.md)

[原文](https://research.google/pubs/mastering-atari-with-discrete-world-models/) · [PDF](https://arxiv.org/pdf/2010.02193) · [阅读卡片](../../../library/dreamerv2.md)

## 机制简析

将世界模型潜状态换成离散表示，利用想象轨迹训练策略，重点检查Atari学习表现。

带着这个问题读：离散潜变量怎样帮助世界模型预测和想象？

初读判断：离散表征和优化设计有清楚前后对照；任务范围保留Atari。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 88 | 20% |
| 实验与证据 | 89 | 20% |
| 学术影响 | 39.2 | 10% |
| 近期关注 | 17.7 | 5% |
| 复用价值 | 91 | 8% |
| 阅读价值 | 91 | 7% |

刊会依据：[ICLR 2021](../../../venues/ICLR/README.md)，正式出处见[出版/原文记录](https://research.google/pubs/mastering-atari-with-discrete-world-models/)；采用2026-10-10刊会快照。


编辑深度：选题初读；评分记录：2026-10-10。

计量版本：作者预印本；OpenAlex题目：Mastering Atari with Discrete World Models。累计被引 22，2025–2026 被引 2；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W3091507139) · [文献计量条目](https://openalex.org/W3091507139)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
