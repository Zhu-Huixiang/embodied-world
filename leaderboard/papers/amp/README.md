# AMP: Adversarial Motion Priors for Stylized Physics-Based Character Control

**AMP** · SIGGRAPH / TOG 2021 · 本版排名 30 · 综合分 **89.2 / 100**

[原文](https://xbpeng.github.io/projects/AMP/) · [PDF](https://xbpeng.github.io/projects/AMP/AMP_2021.pdf) · [阅读卡片](../../../library/amp.md)

## 机制简析

判别器区分参考与策略动作转移，把模仿先验变成奖励，减少逐帧跟踪的限制。

带着这个问题读：判别器学到的动作先验，怎样替代逐帧跟踪奖励？

初读判断：动作先验与任务奖励的解耦影响后续控制，原作任务仍是物理角色。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 90.4 | 30% |
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
