# Mastering Atari with Discrete World Models

**DreamerV2** · ICLR 2021 · 本版排名 87 · 综合分 **82.0 / 100**

[解读导读](../../../library/dreamerv2.md) · [世界模型与模型强化学习](../../../paper-map/README.md#track-world-model) · [ICLR集锦](../../../venues/ICLR/README.md)

[原文](https://research.google/pubs/mastering-atari-with-discrete-world-models/) · [PDF](https://arxiv.org/pdf/2010.02193) · [阅读卡片](../../../library/dreamerv2.md)

论文出处：[**Danijar Hafner**](../../origins/papers/dreamerv2.md)<br>[谷歌研究院 / 谷歌 DeepMind · 另1个机构](../../origins/papers/dreamerv2.md)

## 机制简析

将世界模型潜状态换成离散表示，利用想象轨迹训练策略，重点检查Atari学习表现。

带着这个问题读：离散潜变量怎样帮助世界模型预测和想象？

初读判断：离散表征和优化设计有清楚前后对照；任务范围保留Atari。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 88 | 20% |
| 实验与证据 | 89 | 20% |
| 学术影响 | 39.2 | 10% |
| 近期关注 | 10.0 | 5% |
| 复用价值 | 91 | 8% |
| 阅读价值 | 91 | 7% |

刊会依据：[ICLR 2021](../../../venues/ICLR/README.md)，正式出处见[出版/原文记录](https://research.google/pubs/mastering-atari-with-discrete-world-models/)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：选题初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本；匹配题目：Mastering Atari with Discrete World Models。累计被引 **22**，2025–2026 被引 **2**；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W3091507139) · [文献计量条目](https://openalex.org/W3091507139)

### 影响与关注的计算依据

- **学术影响 39.2**：身份匹配的累计引用C=22，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W3091507139)
- **近期关注 10.0**：近期已定位引用R=2；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W3091507139)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/danijar/dreamerv2) | GitHub Star 1062；GitHub Watch订阅 24；GitHub Fork 212 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [github](https://github.com/jsikyoon/dreamer-torch) | GitHub Star 143；GitHub Watch订阅 1；GitHub Fork 23 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [github](https://github.com/jurgisp/pydreamer) | GitHub Star 240；GitHub Watch订阅 3；GitHub Fork 54 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2010.02193) | HF 论文累计点赞 0 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
