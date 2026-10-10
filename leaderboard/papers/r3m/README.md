# R3M: A Universal Visual Representation for Robot Manipulation

**R3M** · CoRL 2022 · 本版排名 65 · 综合分 **84.5 / 100**

[原文](https://proceedings.mlr.press/v205/nair23a.html) · [PDF](https://proceedings.mlr.press/v205/nair23a/nair23a.pdf) · [阅读卡片](../../../library/r3m.md)

## 机制简析

在人类视频上联合时间对比、视频语言对齐和稀疏约束，让编码器同时记住场景变化与任务语义。下游冻结编码器，把图像向量交给机器人策略，只用少量机器人示范学习动作。原文比较从零训练、CLIP、MoCo 等视觉初始化，并在真实公寓中测试操作。

带着这个问题读：人类第一视角视频里学来的视觉表征，怎样成为机器人少样本操作的感知模块？

初读判断：CoRL 正式版提供三种目标、多个仿真任务和真实少示范对照，公开预训练模型；后续 VC-1 系统研究把 R3M 列为核心对照。

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
| 学术影响 | 54.9 | 10% |
| 近期关注 | 42.5 | 5% |
| 复用价值 | 97 | 8% |
| 阅读价值 | 93 | 7% |

刊会依据：[CoRL 2022](../../../venues/CoRL/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v205/nair23a.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：R3M: A Universal Visual Representation for Robot Manipulation。累计被引 80，2025–2026 被引 13；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4221159977) · [文献计量条目](https://openalex.org/W4221159977)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
