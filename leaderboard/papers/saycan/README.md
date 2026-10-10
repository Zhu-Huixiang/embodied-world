# Do As I Can, Not As I Say: Grounding Language in Robotic Affordances

**SayCan** · CoRL 2022 · 本版排名 35 · 综合分 **88.4 / 100**

[原文](https://proceedings.mlr.press/v205/ichter23a.html) · [PDF](https://proceedings.mlr.press/v205/ichter23a/ichter23a.pdf) · [阅读卡片](../../../library/saycan.md)

## 机制简析

高层指令与已执行步骤送给语言模型，为每个候选技能估计它对任务的适用性；技能价值函数再估计当前场景下的执行成功可能。两者合并后选择技能、实际执行并把步骤加入上下文，直到选出结束。原文分开报告计划与执行，因而能看清语言推理和物理技能各自卡在哪里。

带着这个问题读：语言模型觉得该做的事，机器人做得到吗？两个概率相乘到底解决什么？

初读判断：PMLR 正式论文与项目页给出真实厨房任务、语言模型替换、可供性约束实例及开源桌面版；创新是接口与组合机制，低层技能仍是独立预训练模块。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 90.0 | 30% |
| 创新性 | 94 | 20% |
| 实验与证据 | 89 | 20% |
| 学术影响 | 78.0 | 10% |
| 近期关注 | 78.8 | 5% |
| 复用价值 | 79 | 8% |
| 阅读价值 | 96 | 7% |

刊会依据：[CoRL 2022](../../../venues/CoRL/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v205/ichter23a.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：Do As I Can, Not As I Say: Grounding Language in Robotic Affordances。累计被引 515，2025–2026 被引 133；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4224912544) · [文献计量条目](https://openalex.org/W4224912544)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
