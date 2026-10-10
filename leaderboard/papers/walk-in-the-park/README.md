# Demonstrating A Walk in the Park: Learning to Walk in 20 Minutes With Model-Free Reinforcement Learning

**Walk in the Park** · RSS 2023 · 本版排名 57 · 综合分 **85.3 / 100**

[原文](https://www.roboticsproceedings.org/rss19/p056.html) · [PDF](https://www.roboticsproceedings.org/rss19/p056.pdf) · [阅读卡片](../../../library/walk-in-the-park.md)

## 机制简析

基于 SAC/DroQ 的 actor-critic 从实机回放数据学习，用较高更新比、Dropout 和归一化稳定值函数。策略直接输出关节目标，本体传感器提供状态和奖励，异步采样训练与仔细的动作空间设计减少等待。论文在室内外多种地面验证从头学走路，并在模拟中分析设计选择。

带着这个问题读：没有世界模型和动作模板，如何把实机采样与梯度更新快到足够实用？

初读判断：RSS 正式论文，有真实在线学习、多地面实验和算法/系统设计分析；可与世界模型实机路线作有条件的技术比较。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 86 | 20% |
| 实验与证据 | 91 | 20% |
| 学术影响 | 49.3 | 10% |
| 近期关注 | 51.1 | 5% |
| 复用价值 | 91 | 8% |
| 阅读价值 | 95 | 7% |

刊会依据：[RSS 2023](../../../venues/RSS/README.md)，正式出处见[出版/原文记录](https://www.roboticsproceedings.org/rss19/p056.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：Demonstrating A Walk in the Park: Learning to Walk in 20 Minutes With Model-Free Reinforcement Learning。累计被引 51，2025–2026 被引 23；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W4385430550) · [文献计量条目](https://openalex.org/W4385430550)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
