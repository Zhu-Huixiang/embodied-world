# Demonstrating A Walk in the Park: Learning to Walk in 20 Minutes With Model-Free Reinforcement Learning

**Walk in the Park** · RSS 2023 · 本版排名 64 · 综合分 **84.5 / 100**

[解读导读](../../../library/walk-in-the-park.md) · [Locomotion 与运动适应](../../../paper-map/README.md#track-locomotion) · [RSS集锦](../../../venues/RSS/README.md)

[原文](https://www.roboticsproceedings.org/rss19/p056.html) · [PDF](https://www.roboticsproceedings.org/rss19/p056.pdf) · [阅读卡片](../../../library/walk-in-the-park.md)

论文出处：[**Laura Smith / Ilya Kostrikov**](../../origins/papers/walk-in-the-park.md)<br>[伯克利 BAIR 实验室](../../origins/papers/walk-in-the-park.md)

## 机制简析

基于 SAC/DroQ 的 actor-critic 从实机回放数据学习，用较高更新比、Dropout 和归一化稳定值函数。策略直接输出关节目标，本体传感器提供状态和奖励，异步采样训练与仔细的动作空间设计减少等待。论文在室内外多种地面验证从头学走路，并在模拟中分析设计选择。

带着这个问题读：没有世界模型和动作模板，如何把实机采样与梯度更新快到足够实用？

初读判断：RSS 正式论文，有真实在线学习、多地面实验和算法/系统设计分析；可与世界模型实机路线作有条件的技术比较。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 86 | 20% |
| 实验与证据 | 91 | 20% |
| 学术影响 | 49.3 | 10% |
| 近期关注 | 34.9 | 5% |
| 复用价值 | 91 | 8% |
| 阅读价值 | 95 | 7% |

刊会依据：[RSS 2023](../../../venues/RSS/README.md)，正式出处见[出版/原文记录](https://www.roboticsproceedings.org/rss19/p056.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：Demonstrating A Walk in the Park: Learning to Walk in 20 Minutes With Model-Free Reinforcement Learning。累计被引 **51**，2025–2026 被引 **23**；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W4385430550) · [文献计量条目](https://openalex.org/W4385430550)

### 影响与关注的计算依据

- **学术影响 49.3**：身份匹配的累计引用C=51，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4385430550)
- **近期关注 34.9**：近期已定位引用R=23；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W4385430550)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/ikostrikov/walk_in_the_park) | GitHub Star 284；GitHub Watch订阅 9；GitHub Fork 39 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
