# Learning to Walk in Minutes Using Massively Parallel Deep Reinforcement Learning

**Legged Gym** · CoRL 2021 · 本版排名 69 · 综合分 **83.9 / 100**

[原文](https://proceedings.mlr.press/v164/rudin22a.html) · [PDF](https://proceedings.mlr.press/v164/rudin22a/rudin22a.pdf) · [阅读卡片](../../../library/walk-in-minutes.md)

## 机制简析

物理仿真和 PPO 训练都留在 GPU 上，用大量并行环境快速组成更新批次。地形课程根据机器人前进表现升降难度，任务课程逐步扩大命令范围。原文分析大并行下训练组件并把 ANYmal 策略转到实机，公开 legged_gym。

带着这个问题读：把几千只机器人放到同一块 GPU，训练速度与课程怎么一起改变？

初读判断：有训练设置分析、课程与 sim-to-real 实验；公开代码是复用入口，后续 Extreme Parkour 原文直接比较该工作。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 90.0 | 30% |
| 创新性 | 88 | 20% |
| 实验与证据 | 90 | 20% |
| 学术影响 | 48.9 | 10% |
| 近期关注 | 40.0 | 5% |
| 复用价值 | 98 | 8% |
| 阅读价值 | 94 | 7% |

刊会依据：[CoRL 2021](../../../venues/CoRL/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v164/rudin22a.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：Learning to Walk in Minutes Using Massively Parallel Deep Reinforcement Learning。累计被引 49，2025–2026 被引 11；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W3200962355) · [文献计量条目](https://openalex.org/W3200962355)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
