# Planning with Diffusion for Flexible Behavior Synthesis

**Diffuser** · ICML 2022 · 本版排名 54 · 综合分 **85.3 / 100**

[解读导读](../../../library/diffuser.md) · [世界动作模型](../../../paper-map/README.md#track-world-action-model) · [ICML集锦](../../../venues/ICML/README.md)

[原文](https://proceedings.mlr.press/v162/janner22a.html) · [PDF](https://proceedings.mlr.press/v162/janner22a/janner22a.pdf) · [阅读卡片](../../../library/diffuser.md)

论文出处：[Michael Janner / Yilun Du · UC Berkeley / MIT](../../origins/papers/diffuser.md)

## 机制简析

Diffuser 学习整段状态—动作轨迹的去噪过程，反复修正所有规划时刻，而不是单步滚动一个动力学模型。奖励梯度可以引导去噪，固定起点或终点则像图像补全那样锁住轨迹部分。论文在长时序与灵活测试条件下比较规划效果，并区分扩散步和环境时间步。

带着这个问题读：轨迹一起去噪，如何同时承担环境建模、长时序规划与测试时加约束？

初读判断：提出可组合的生成式规划框架，有长时序控制及条件变化实验，正式 ICML 论文和官方项目可复核。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 95 | 20% |
| 实验与证据 | 85 | 20% |
| 学术影响 | 50.9 | 10% |
| 近期关注 | 28.2 | 5% |
| 复用价值 | 94 | 8% |
| 阅读价值 | 97 | 7% |

刊会依据：[ICML 2022](../../../venues/ICML/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v162/janner22a.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：Planning with Diffusion for Flexible Behavior Synthesis。累计被引 **58**，2025–2026 被引 **14**；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W4281398962) · [文献计量条目](https://openalex.org/W4281398962)

### 影响与关注的计算依据

- **学术影响 50.9**：身份匹配的累计引用C=58，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4281398962)
- **近期关注 28.2**：近期已定位引用R=14；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W4281398962)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/jannerm/diffuser) | GitHub Star 1311；GitHub Watch订阅 12；GitHub Fork 200 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2205.09991) | HF 论文累计点赞 3；HF 论文讨论评论累计数 1 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
