# AMP: Adversarial Motion Priors for Stylized Physics-Based Character Control

本版阅读优先顺序：29；综合分：89.2 / 100；已评分权重：100%。

[原文](https://xbpeng.github.io/projects/AMP/) · [PDF](https://xbpeng.github.io/projects/AMP/AMP_2021.pdf) · [阅读卡片](../../../library/amp.md)

## 机制简析

判别器区分参考与策略动作转移，把模仿先验变成奖励，减少逐帧跟踪的限制。

带着这个问题读：判别器学到的动作先验，怎样替代逐帧跟踪奖励？

初读判断：动作先验与任务奖励的解耦影响后续控制，原作任务仍是物理角色。

## 七维评分

![七维雷达：加载时展开一次，随后静止](radar.gif)

打开时从中心展开一次，结束后保持最终形状。[直接查看静态图](radar.svg)。加载与再次打开的播放时机取决于浏览器缓存。

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 刊会质量 | 90.4 | 30% |
| 创新性 | 94 | 20% |
| 实验与证据 | 88 | 20% |
| 学术影响 | 74.7 | 10% |
| 近期关注 | 83.4 | 5% |
| 复用价值 | 90 | 8% |
| 阅读价值 | 97 | 7% |

刊会依据：[SIGGRAPH / TOG 2021](../../../venues/SIGGRAPH-TOG/README.md)，正式出处见[出版/原文记录](https://xbpeng.github.io/projects/AMP/)；采用2026-10-10刊会快照。


编辑深度：选题初读；评分记录：2026-10-10。

计量版本：正式刊会版本；OpenAlex题目：AMP。累计被引 394，2025–2026 被引 177；快照：2026-10-09T18:48:09+08:00。

[指标记录](https://api.openalex.org/works/W3147968035) · [文献计量条目](https://openalex.org/W3147968035)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
