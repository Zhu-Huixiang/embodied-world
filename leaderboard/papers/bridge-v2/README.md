# BridgeData V2: A Dataset for Robot Learning at Scale

**BridgeData V2** · CoRL 2023 · 本版排名 92 · 综合分 **80.5 / 100**

[解读导读](../../../library/bridge-v2.md) · [操作与动作块](../../../paper-map/README.md#track-manipulation) · [CoRL集锦](../../../venues/CoRL/README.md)

[原文](https://proceedings.mlr.press/v229/walke23a.html) · [PDF](https://proceedings.mlr.press/v229/walke23a/walke23a.pdf) · [阅读卡片](../../../library/bridge-v2.md)

## 机制简析

统一低成本机械臂平台收集语言标注轨迹，同时主动变化物体、相机、场景和工作台位置。策略可按目标图或自然语言训练，测试再拆开已见任务的视觉变化与新物体、新环境泛化。不同离线学习方法、数据规模和模型容量在同一数据上比较，让数据多样性的作用有可检查的落点。

带着这个问题读：机器人数据怎样覆盖场景差异，才会支持跨环境与跨机构技能迁移？

初读判断：CoRL 正式版与项目提供多环境数据、多个离线算法及数据/容量研究，开放数据、预训练模型和硬件指南复用价值很高；贡献主要在可泛化数据基础设施。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 90.0 | 30% |
| 创新性 | 84 | 20% |
| 实验与证据 | 91 | 20% |
| 学术影响 | 32.0 | 10% |
| 近期关注 | 22.3 | 5% |
| 复用价值 | 99 | 8% |
| 阅读价值 | 90 | 7% |

刊会依据：[CoRL 2023](../../../venues/CoRL/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v229/walke23a.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：BridgeData V2: A Dataset for Robot Learning at Scale。累计被引 12，2025–2026 被引 3；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4386185624) · [文献计量条目](https://openalex.org/W4386185624)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
