# RT-1: Robotics Transformer for Real-World Control at Scale

本版阅读优先顺序：16；综合分：91.7 / 100；已评分权重：100%。

[原文](https://www.roboticsproceedings.org/rss19/p025.html) · [PDF](https://roboticsproceedings.org/rss19/p025.pdf) · [阅读卡片](../../../library/rt1.md)

## 机制简析

图像先经语言条件的 EfficientNet 提取特征，再由 TokenLearner 压成少量视觉 token；Transformer 融合短时历史并输出离散动作。动作同时覆盖机械臂、底盘和停止模式，策略以闭环方式反复读取图像。原文分别检验新指令、干扰物、新背景以及跨机器人数据混合的效果。

带着这个问题读：大量真实机器人数据究竟需要什么策略结构才能吃进去，TokenLearner 为何是关键？

初读判断：RSS 正式 PDF 与项目页给出 BC-Z、Gato 对照、数据量/数据多样性消融和真实厨房评估，证据丰富；开源模型和数据提供复用入口。

## 七维评分

![七维雷达：加载时展开一次，随后静止](radar.gif)

打开时从中心展开一次，结束后保持最终形状。[直接查看静态图](radar.svg)。加载与再次打开的播放时机取决于浏览器缓存。

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 刊会质量 | 95.0 | 30% |
| 创新性 | 91 | 20% |
| 实验与证据 | 92 | 20% |
| 学术影响 | 80.9 | 10% |
| 近期关注 | 98.8 | 5% |
| 复用价值 | 86 | 8% |
| 阅读价值 | 95 | 7% |

刊会依据：[RSS 2023](../../../venues/RSS/README.md)，正式出处见[出版/原文记录](https://www.roboticsproceedings.org/rss19/p025.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：RT-1: Robotics Transformer for Real-World Control at Scale。累计被引 651，2025–2026 被引 464；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4385430679) · [文献计量条目](https://openalex.org/W4385430679)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
