# Planning with Diffusion for Flexible Behavior Synthesis

本版阅读优先顺序：48；综合分：86.1 / 100；已评分权重：100%。

[原文](https://proceedings.mlr.press/v162/janner22a.html) · [PDF](https://proceedings.mlr.press/v162/janner22a/janner22a.pdf) · [阅读卡片](../../../library/diffuser.md)

## 机制简析

Diffuser 学习整段状态—动作轨迹的去噪过程，反复修正所有规划时刻，而不是单步滚动一个动力学模型。奖励梯度可以引导去噪，固定起点或终点则像图像补全那样锁住轨迹部分。论文在长时序与灵活测试条件下比较规划效果，并区分扩散步和环境时间步。

带着这个问题读：轨迹一起去噪，如何同时承担环境建模、长时序规划与测试时加约束？

初读判断：提出可组合的生成式规划框架，有长时序控制及条件变化实验，正式 ICML 论文和官方项目可复核。

## 七维评分

![七维雷达：加载时展开一次，随后静止](radar.gif)

打开时从中心展开一次，结束后保持最终形状。[直接查看静态图](radar.svg)。加载与再次打开的播放时机取决于浏览器缓存。

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 刊会质量 | 95.0 | 30% |
| 创新性 | 95 | 20% |
| 实验与证据 | 85 | 20% |
| 学术影响 | 50.9 | 10% |
| 近期关注 | 43.6 | 5% |
| 复用价值 | 94 | 8% |
| 阅读价值 | 97 | 7% |

刊会依据：[ICML 2022](../../../venues/ICML/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v162/janner22a.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：Planning with Diffusion for Flexible Behavior Synthesis。累计被引 58，2025–2026 被引 14；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W4281398962) · [文献计量条目](https://openalex.org/W4281398962)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
