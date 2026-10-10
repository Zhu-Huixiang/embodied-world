# EfficientZero V2: Mastering Discrete and Continuous Control with Limited Data

本版阅读优先顺序：93；综合分：75.0 / 100；已评分权重：100%。

[原文](https://proceedings.mlr.press/v235/wang24at.html) · [PDF](https://raw.githubusercontent.com/mlresearch/v235/main/assets/wang24at/wang24at.pdf) · [阅读卡片](../../../library/efficientzero-v2.md)

## 机制简析

表示函数得到潜状态，动力学函数接收动作并预测潜状态与奖励，策略和值网络为搜索提供先验。连续动作下先采样候选动作，再用基于 Gumbel 的树搜索改善策略，并用搜索产生价值目标以利用旧经验。实验按有限交互预算比较离散和连续、图像和低维输入任务。

带着这个问题读：树搜索怎样跨过离散动作的限制，在连续控制里仍保持样本效率？

初读判断：正式 ICML Spotlight，原文跨三类基准并比较 DreamerV3；连续树搜索与价值估计分别有消融，初读评分保留为编辑判断。

## 七维评分

![七维雷达：加载时展开一次，随后静止](radar.gif)

打开时从中心展开一次，结束后保持最终形状。[直接查看静态图](radar.svg)。加载与再次打开的播放时机取决于浏览器缓存。

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 刊会质量 | 95.0 | 30% |
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
