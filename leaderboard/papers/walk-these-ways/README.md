# Walk These Ways: Tuning Robot Control for Generalization with Multiplicity of Behavior

**Walk These Ways** · CoRL 2022 · 本版排名 85 · 综合分 **81.4 / 100**

[原文](https://proceedings.mlr.press/v205/margolis23a.html) · [PDF](https://proceedings.mlr.press/v205/margolis23a/margolis23a.pdf) · [阅读卡片](../../../library/walk-these-ways.md)

## 机制简析

一个策略同时接收三维速度命令和八维行为参数，后者控制足端相位、频率、身体姿态与抬脚等走法。历史本体观测与这些命令共同输入网络，输出十二个关节的位置目标。测试时人可以调整行为参数，在不重训情况下为新任务挑选合适步态。

带着这个问题读：遇到新地面不重训，能否直接调一组步态参数让同一个策略换种走法？

初读判断：可调参数定义清楚，有实机多行为、能耗和分布外任务比较，公开控制器使读者能够继续实验。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 90.0 | 30% |
| 创新性 | 87 | 20% |
| 实验与证据 | 87 | 20% |
| 学术影响 | 37.4 | 10% |
| 近期关注 | 35.3 | 5% |
| 复用价值 | 96 | 8% |
| 阅读价值 | 92 | 7% |

刊会依据：[CoRL 2022](../../../venues/CoRL/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v205/margolis23a.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：Walk These Ways: Tuning Robot Control for Generalization with Multiplicity of Behavior。累计被引 19，2025–2026 被引 8；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W4310886200) · [文献计量条目](https://openalex.org/W4310886200)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
