# HumanPlus: Humanoid Shadowing and Imitation from Humans

**HumanPlus** · CoRL 2024 · 本版排名 91 · 综合分 **80.5 / 100**

[原文](https://proceedings.mlr.press/v270/fu25a.html) · [PDF](https://raw.githubusercontent.com/mlresearch/v270/main/assets/fu25a/fu25a.pdf) · [阅读卡片](../../../library/humanplus.md)

## 机制简析

用人类运动重定向数据在模拟里训练姿态条件的低层控制，再用单 RGB 相机估计操作者姿态，让实机实时跟随。跟随过程中记录机器人双目视觉和全身动作，随后用 Humanoid Imitation Transformer 做监督模仿，得到自主任务策略。原文分别评估遥操作、抗扰和多项自主任务。

带着这个问题读：人做动作、机器人跟动作、再学自主任务，这三段数据链路如何接起来？

初读判断：正式 CoRL，有真实人形、遥操作对照和任务成功率；同时覆盖全身控制与数据采集，适合正式公众号的系统解读。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 90.0 | 30% |
| 创新性 | 91 | 20% |
| 实验与证据 | 90 | 20% |
| 学术影响 | 22.4 | 10% |
| 近期关注 | 22.3 | 5% |
| 复用价值 | 90 | 8% |
| 阅读价值 | 97 | 7% |

刊会依据：[CoRL 2024](../../../venues/CoRL/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v270/fu25a.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：HumanPlus: Humanoid Shadowing and Imitation from Humans。累计被引 5，2025–2026 被引 3；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W4399794218) · [文献计量条目](https://openalex.org/W4399794218)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
