# DeepMimic: Example-Guided Deep Reinforcement Learning of Physics-Based Character Skills

**DeepMimic** · SIGGRAPH / TOG 2018 · 本版排名 21 · 综合分 **90.8 / 100**

[解读导读](../../../library/deepmimic.md) · [动作先验与全身技能](../../../paper-map/README.md#track-motion-priors) · [SIGGRAPH / TOG集锦](../../../venues/SIGGRAPH-TOG/README.md)

[原文](https://xbpeng.github.io/projects/DeepMimic/) · [PDF](https://xbpeng.github.io/projects/DeepMimic/DeepMimic_2018.pdf) · [阅读卡片](../../../library/deepmimic.md)

## 机制简析

任务奖励与参考动作跟踪奖励共同训练物理角色策略，使动作技能能在动态扰动后恢复。

带着这个问题读：模仿奖励与任务奖励怎样把动作片段变成可恢复的控制技能？

初读判断：示范驱动物理控制的基础路线；公开实现利于机制实验。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 90.4 | 30% |
| 创新性 | 96 | 20% |
| 实验与证据 | 88 | 20% |
| 学术影响 | 85.1 | 10% |
| 近期关注 | 85.8 | 5% |
| 复用价值 | 93 | 8% |
| 阅读价值 | 95 | 7% |

刊会依据：[SIGGRAPH / TOG 2018](../../../venues/SIGGRAPH-TOG/README.md)，正式出处见[出版/原文记录](https://xbpeng.github.io/projects/DeepMimic/)；采用2026-10-10刊会快照。


编辑深度：选题初读；评分记录：2026-10-10。

计量版本：正式刊会版本；OpenAlex题目：DeepMimic。累计被引 906，2025–2026 被引 206；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W2796290181) · [文献计量条目](https://openalex.org/W2796290181)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
