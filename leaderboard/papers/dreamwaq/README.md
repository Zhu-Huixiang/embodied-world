# DreamWaQ: Learning Robust Quadrupedal Locomotion With Implicit Terrain Imagination via Deep Reinforcement Learning

**DreamWaQ** · ICRA 2023 · 本版排名 84 · 综合分 **82.2 / 100**

[解读导读](../../../library/dreamwaq.md) · [Locomotion 与运动适应](../../../paper-map/README.md#track-locomotion) · [ICRA集锦](../../../venues/ICRA/README.md)

[原文](https://ieeexplore.ieee.org/abstract/document/10161144/) · [PDF](https://arxiv.org/pdf/2301.10602) · [阅读卡片](../../../library/dreamwaq.md)

论文出处：[I Made Aswin Nahrendra · Korea Advanced Institute of Science and Technology](../../origins/papers/dreamwaq.md)

## 机制简析

从本体历史估计速度和隐环境表示，将其送给策略；训练时以重建/特权监督组织环境编码。

带着这个问题读：盲行走时，历史本体信息怎样形成环境表征并进入 actor？

初读判断：盲行走的历史表征与actor连接清楚；越障和地形条件是精读重点。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 83.0 | 30% |
| 创新性 | 86 | 20% |
| 实验与证据 | 87 | 20% |
| 学术影响 | 63.4 | 10% |
| 近期关注 | 63.6 | 5% |
| 复用价值 | 83 | 8% |
| 阅读价值 | 93 | 7% |

刊会依据：[ICRA 2023](../../../venues/ICRA/README.md)，正式出处见[出版/原文记录](https://ieeexplore.ieee.org/abstract/document/10161144/)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：选题初读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：DreamWaQ: Learning Robust Quadrupedal Locomotion With Implicit Terrain Imagination via Deep Reinforcement Learning。累计被引 **159**，2025–2026 被引 **126**；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W4383108274) · [文献计量条目](https://openalex.org/W4383108274)

### 影响与关注的计算依据

- **学术影响 63.4**：身份匹配的累计引用C=159，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4383108274)
- **近期关注 63.6**：近期已定位引用R=126；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W4383108274)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/curieuxjy/go2_dreamwaq) | GitHub Star 34；GitHub Watch订阅 1；GitHub Fork 5 | 多论文/多模型共享仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2301.10602) | HF 论文累计点赞 0 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
