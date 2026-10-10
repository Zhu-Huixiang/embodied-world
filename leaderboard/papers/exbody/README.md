# Expressive Whole-Body Control for Humanoid Robots

**ExBody** · RSS 2024 · 本版排名 44 · 综合分 **86.7 / 100**

[解读导读](../../../library/exbody.md) · [Locomotion 与运动适应](../../../paper-map/README.md#track-locomotion) · [RSS集锦](../../../venues/RSS/README.md)

[原文](https://www.roboticsproceedings.org/rss20/p107.html) · [PDF](https://www.roboticsproceedings.org/rss20/p107.pdf) · [阅读卡片](../../../library/exbody.md)

## 机制简析

从人类动作库筛选并重定向姿态，训练时要求机器人上半身跟随关节和关键点目标。下半身放松逐关节模仿约束，改为跟随根速度和姿态命令，以留出平衡和行走空间。原文对照完整身体跟踪、分开策略与初始化方式，实机展示行走和表达动作。

带着这个问题读：上半身想照着人动，下半身还得站稳，这两种目标怎么兼容？

初读判断：正式 RSS，核心约束改动与完整跟踪基线直接比较，sim-to-real 与实机动作支持其科学问题。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 87 | 20% |
| 实验与证据 | 89 | 20% |
| 学术影响 | 56.3 | 10% |
| 近期关注 | 70.1 | 5% |
| 复用价值 | 91 | 8% |
| 阅读价值 | 94 | 7% |

刊会依据：[RSS 2024](../../../venues/RSS/README.md)，正式出处见[出版/原文记录](https://www.roboticsproceedings.org/rss20/p107.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：Expressive Whole-Body Control for Humanoid Robots。累计被引 90，2025–2026 被引 77；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W4402354017) · [文献计量条目](https://openalex.org/W4402354017)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
