# ASE: Large-Scale Reusable Adversarial Skill Embeddings for Physically Simulated Characters

本版阅读优先顺序：25；综合分：75.7–90.7 / 100；已评分权重：85%。

[原文](https://xbpeng.github.io/projects/ASE/) · [PDF](https://xbpeng.github.io/projects/ASE/ASE_2022.pdf) · [阅读卡片](../../../library/ase.md)

## 机制简析

将潜技能条件与对抗动作先验联合训练，再让高层策略选择可复用的技能嵌入。

带着这个问题读：连续技能潜变量怎样组织可重复使用的动作？

初读判断：可复用技能接口值得与机器人动作latent比较；初读分清训练奖励和高层控制。

## 七维评分

![七维雷达：加载时展开一次，随后静止](radar.gif)

打开时从中心展开一次，结束后保持最终形状。[直接查看静态图](radar.svg)。加载与再次打开的播放时机取决于浏览器缓存。

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 刊会质量 | 90.4 | 30% |
| 创新性 | 90 | 20% |
| 实验与证据 | 86 | 20% |
| 学术影响 | 待核验 | 10% |
| 近期关注 | 待核验 | 5% |
| 复用价值 | 88 | 8% |
| 阅读价值 | 91 | 7% |

刊会依据：[SIGGRAPH / TOG 2022](../../../venues/SIGGRAPH-TOG/README.md)，正式出处见[出版/原文记录](https://xbpeng.github.io/projects/ASE/)；采用2026-10-09刊会快照。


编辑深度：选题初读；评分记录：2026-10-09T18:35:28+08:00。

计量状态：等待可确认对应的记录；两项计量维度保留空白。

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
