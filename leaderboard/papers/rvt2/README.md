# RVT-2: Learning Precise Manipulation from Few Demonstrations

本版阅读优先顺序：49；综合分：85.8 / 100；已评分权重：100%。

[原文](https://www.roboticsproceedings.org/rss20/p055.html) · [PDF](https://www.roboticsproceedings.org/rss20/p055.pdf) · [阅读卡片](../../../library/rvt2.md)

## 机制简析

第一阶段在全场景虚拟视图中估计目标，第二阶段放大局部区域后预测更精确的位置；旋转预测改用目标位置附近特征，避免同场景多个物体方向冲突。凸上采样、较少视图和高效点云渲染控制计算成本。原文分别做这些部件的消融，并用插头和不同孔径 peg 的实机任务检验精度。

带着这个问题读：粗视图定位之后再放大，怎样改善毫米级插入，而不是只让网络更快？

初读判断：RSS PDF 提供粗到细结构、位置条件旋转和系统优化消融，以及十示范量级的实机精密任务；属于高质量迭代而非全新范式，因此创新分适度。

## 七维评分

![七维雷达：加载时展开一次，随后静止](radar.gif)

打开时从中心展开一次，结束后保持最终形状。[直接查看静态图](radar.svg)。加载与再次打开的播放时机取决于浏览器缓存。

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 刊会质量 | 95.0 | 30% |
| 创新性 | 86 | 20% |
| 实验与证据 | 91 | 20% |
| 学术影响 | 48.6 | 10% |
| 近期关注 | 62.6 | 5% |
| 复用价值 | 94 | 8% |
| 阅读价值 | 91 | 7% |

刊会依据：[RSS 2024](../../../venues/RSS/README.md)，正式出处见[出版/原文记录](https://www.roboticsproceedings.org/rss20/p055.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：RVT-2: Learning Precise Manipulation from Few Demonstrations。累计被引 48，2025–2026 被引 48；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4402354093) · [文献计量条目](https://openalex.org/W4402354093)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
