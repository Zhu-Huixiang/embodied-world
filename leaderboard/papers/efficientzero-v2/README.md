# EfficientZero V2: Mastering Discrete and Continuous Control with Limited Data

**EfficientZero V2** · ICML 2024 · 本版排名 101 · 综合分 **75.0 / 100**

[解读导读](../../../library/efficientzero-v2.md) · [世界模型与模型强化学习](../../../paper-map/README.md#track-world-model) · [ICML集锦](../../../venues/ICML/README.md)

[原文](https://proceedings.mlr.press/v235/wang24at.html) · [PDF](https://raw.githubusercontent.com/mlresearch/v235/main/assets/wang24at/wang24at.pdf) · [阅读卡片](../../../library/efficientzero-v2.md)

## 机制简析

表示函数得到潜状态，动力学函数接收动作并预测潜状态与奖励，策略和值网络为搜索提供先验。连续动作下先采样候选动作，再用基于 Gumbel 的树搜索改善策略，并用搜索产生价值目标以利用旧经验。实验按有限交互预算比较离散和连续、图像和低维输入任务。

带着这个问题读：树搜索怎样跨过离散动作的限制，在连续控制里仍保持样本效率？

初读判断：正式 ICML Spotlight，原文跨三类基准并比较 DreamerV3；连续树搜索与价值估计分别有消融，初读评分保留为编辑判断。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 84 | 20% |
| 实验与证据 | 87 | 20% |
| 学术影响 | 0.0 | 10% |
| 近期关注 | 0.0 | 5% |
| 复用价值 | 78 | 8% |
| 阅读价值 | 87 | 7% |

刊会依据：[ICML 2024](../../../venues/ICML/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v235/wang24at.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：EfficientZero V2: Mastering Discrete and Continuous Control with Limited Data。累计被引 0，2025–2026 被引 0；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W4392427796) · [文献计量条目](https://openalex.org/W4392427796)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
