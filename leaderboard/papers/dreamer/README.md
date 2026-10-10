# Dream to Control: Learning Behaviors by Latent Imagination

**Dreamer** · ICLR 2020 · 本版排名 38 · 综合分 **88.1 / 100**

[解读导读](../../../library/dreamer.md) · [世界模型与模型强化学习](../../../paper-map/README.md#track-world-model) · [ICLR集锦](../../../venues/ICLR/README.md)

[原文](https://research.google/pubs/dream-to-control-learning-behaviors-by-latent-imagination/) · [PDF](https://arxiv.org/pdf/1912.01603) · [阅读卡片](../../../library/dreamer.md)

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
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 97 | 20% |
| 实验与证据 | 89 | 20% |
| 学术影响 | 61.0 | 10% |
| 近期关注 | 38.6 | 5% |
| 复用价值 | 94 | 8% |
| 阅读价值 | 98 | 7% |

刊会依据：[ICLR 2020](../../../venues/ICLR/README.md)，正式出处见[出版/原文记录](https://research.google/pubs/dream-to-control-learning-behaviors-by-latent-imagination/)；采用2026-10-10刊会快照。


编辑深度：选题初读；评分记录：2026-10-10。

计量版本：作者预印本；OpenAlex题目：Dream to Control: Learning Behaviors by Latent Imagination。累计被引 131，2025–2026 被引 10；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W2992977009) · [文献计量条目](https://openalex.org/W2992977009)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
