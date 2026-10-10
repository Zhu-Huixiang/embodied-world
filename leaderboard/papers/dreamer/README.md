# Dream to Control: Learning Behaviors by Latent Imagination

**Dreamer** · ICLR 2020 · 本版排名 39 · 综合分 **87.4 / 100**

[解读导读](../../../library/dreamer.md) · [世界模型与模型强化学习](../../../paper-map/README.md#track-world-model) · [ICLR集锦](../../../venues/ICLR/README.md)

[原文](https://research.google/pubs/dream-to-control-learning-behaviors-by-latent-imagination/) · [PDF](https://arxiv.org/pdf/1912.01603) · [阅读卡片](../../../library/dreamer.md)

论文出处：[**Danijar Hafner**](../../origins/papers/dreamer.md)<br>[多伦多大学 / 谷歌研究院 / Brain 团队 · 另1个机构](../../origins/papers/dreamer.md)

## 机制简析

学习潜动力学世界模型，在想象轨迹里以价值反馈优化actor，把像素预测转成决策训练信号。

带着这个问题读：RSSM 如何从观测和动作建模未来，actor 又怎样在潜空间学习？

初读判断：潜空间想象连接模型与策略的基础工作；代码和后续路线利于复用。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 97 | 20% |
| 实验与证据 | 89 | 20% |
| 学术影响 | 61.0 | 10% |
| 近期关注 | 24.2 | 5% |
| 复用价值 | 94 | 8% |
| 阅读价值 | 98 | 7% |

刊会依据：[ICLR 2020](../../../venues/ICLR/README.md)，正式出处见[出版/原文记录](https://research.google/pubs/dream-to-control-learning-behaviors-by-latent-imagination/)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：选题初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本；匹配题目：Dream to Control: Learning Behaviors by Latent Imagination。累计被引 **131**，2025–2026 被引 **10**；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W2992977009) · [文献计量条目](https://openalex.org/W2992977009)

### 影响与关注的计算依据

- **学术影响 61.0**：身份匹配的累计引用C=131，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W2992977009)
- **近期关注 24.2**：近期已定位引用R=10；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W2992977009)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/danijar/dreamer) | GitHub Star 626；GitHub Watch订阅 10；GitHub Fork 121 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/1912.01603) | HF 论文累计点赞 0 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
