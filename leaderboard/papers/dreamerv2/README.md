# Mastering Atari with Discrete World Models

本版阅读优先顺序：21；综合分：82.4 / 100；已评分权重：100%。

[原文](https://research.google/pubs/mastering-atari-with-discrete-world-models/) · [PDF](https://arxiv.org/pdf/2010.02193) · [阅读卡片](../../../library/dreamerv2.md)

## 机制简析

将世界模型潜状态换成离散表示，利用想象轨迹训练策略，重点检查Atari学习表现。

带着这个问题读：离散潜变量怎样帮助世界模型预测和想象？

初读判断：离散表征和优化设计有清楚前后对照；任务范围保留Atari。

## 七维评分

![七维雷达：加载时展开一次，随后静止](radar.gif)

打开时从中心展开一次，结束后保持最终形状。[直接查看静态图](radar.svg)。加载与再次打开的播放时机取决于浏览器缓存。

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 刊会质量 | 95.0 | 30% |
| 创新性 | 88 | 20% |
| 实验与证据 | 89 | 20% |
| 学术影响 | 39.2 | 10% |
| 近期关注 | 17.7 | 5% |
| 复用价值 | 91 | 8% |
| 阅读价值 | 91 | 7% |

刊会依据：[ICLR 2021](../../../venues/ICLR/README.md)，正式出处见[出版/原文记录](https://research.google/pubs/mastering-atari-with-discrete-world-models/)；采用2026-10-09刊会快照。


编辑深度：选题初读；评分记录：2026-10-09T18:35:28+08:00。

计量版本：作者预印本；OpenAlex题目：Mastering Atari with Discrete World Models。累计被引 22，2025–2026 被引 2；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W3091507139) · [文献计量条目](https://openalex.org/W3091507139)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
