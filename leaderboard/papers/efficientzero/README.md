# Mastering Atari Games with Limited Data

本版阅读优先顺序：71；综合分：83.1 / 100；已评分权重：100%。

[原文](https://proceedings.neurips.cc/paper/2021/hash/d5eca8dc3820cad9fe56a3bafda65ca1-Abstract.html) · [PDF](https://proceedings.neurips.cc/paper/2021/file/d5eca8dc3820cad9fe56a3bafda65ca1-Paper.pdf) · [阅读卡片](../../../library/efficientzero.md)

## 机制简析

编码器把图像变成潜状态，动力学网络预测下一潜状态，MCTS 在这个模型里比较动作。EfficientZero 用预测潜状态与真实下一帧编码的一致性补强动力学监督，预测累计价值前缀，并重分析旧数据来缓解离策略目标偏差。它测试的是有限交互预算下的游戏与模拟控制效率。

带着这个问题读：只有少量交互时，潜空间树搜索为什么还需要一致性监督、价值前缀和重分析？

初读判断：有多任务小样本基准、MuZero 对照及组件消融；代码和后续 EfficientZero V2 构成可追踪的复用路线。

## 七维评分

![七维雷达：加载时展开一次，随后静止](radar.gif)

打开时从中心展开一次，结束后保持最终形状。[直接查看静态图](radar.svg)。加载与再次打开的播放时机取决于浏览器缓存。

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 刊会质量 | 95.0 | 30% |
| 创新性 | 89 | 20% |
| 实验与证据 | 87 | 20% |
| 学术影响 | 46.1 | 10% |
| 近期关注 | 25.9 | 5% |
| 复用价值 | 88 | 8% |
| 阅读价值 | 92 | 7% |

刊会依据：[NeurIPS 2021](../../../venues/NeurIPS/README.md)，正式出处见[出版/原文记录](https://proceedings.neurips.cc/paper/2021/hash/d5eca8dc3820cad9fe56a3bafda65ca1-Abstract.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：Mastering Atari Games with Limited Data。累计被引 39，2025–2026 被引 4；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W3208460365) · [文献计量条目](https://openalex.org/W3208460365)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
