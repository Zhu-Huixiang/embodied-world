# CLIPort: What and Where Pathways for Robotic Manipulation

**CLIPort** · CoRL 2021 · 本版排名 61 · 综合分 **85.0 / 100**

[解读导读](../../../library/cliport.md) · [操作与动作块](../../../paper-map/README.md#track-manipulation) · [CoRL集锦](../../../venues/CoRL/README.md)

[原文](https://proceedings.mlr.press/v164/shridhar22a.html) · [PDF](https://proceedings.mlr.press/v164/shridhar22a/shridhar22a.pdf) · [阅读卡片](../../../library/cliport.md)

## 机制简析

语义支路用 CLIP 提取 RGB 与指令概念，空间支路从 RGB-D 学习保持位置结构的特征；两路信息进入 Transporter 的拾取与放置预测。拾取位置先决定裁出哪块特征，再用互相关找到合适的放置区域。原文在多任务仿真和真实桌面上检验新物体、语义概念与少量示范。

带着这个问题读：CLIP 知道是什么，但不知道手该落在哪里；语义和几何怎样配合？

初读判断：PMLR 正式版与作者项目提供双流结构、语义泛化以及真实多任务评估，公开代码支持复用；主题冲突具体且容易讲清。

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
| 实验与证据 | 89 | 20% |
| 学术影响 | 56.5 | 10% |
| 近期关注 | 45.6 | 5% |
| 复用价值 | 92 | 8% |
| 阅读价值 | 96 | 7% |

刊会依据：[CoRL 2021](../../../venues/CoRL/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v164/shridhar22a.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：CLIPort: What and Where Pathways for Robotic Manipulation。累计被引 91，2025–2026 被引 16；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W3203511201) · [文献计量条目](https://openalex.org/W3203511201)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
