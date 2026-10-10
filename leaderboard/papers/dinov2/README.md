# DINOv2: Learning Robust Visual Features without Supervision

本版阅读优先顺序：21；综合分：90.7 / 100；已评分权重：100%。

[原文](https://openreview.net/forum?id=a68SUt6zFt) · [PDF](https://openreview.net/pdf?id=a68SUt6zFt) · [阅读卡片](../../../library/dinov2.md)

## 机制简析

在大规模筛选图像上扩展图像级与 patch 级自监督学习，再把大 ViT 教师蒸馏为不同尺寸的编码器。下游可以冻结 backbone，用轻量预测头读取分类、分割或深度相关信息。原文比较多种图像与像素任务；OpenVLA 的视觉输入实际将 DINOv2 特征与 SigLIP 特征拼接后映射给语言模型。

带着这个问题读：机器人视觉编码器冻结以后，哪些几何和语义信息还能留在 patch 特征里？

初读判断：广泛冻结特征评估、数据与规模设计及开放权重形成很强复用价值；与机器人策略的连接由 OpenVLA 原文确认。

## 七维评分

![七维雷达：加载时展开一次，随后静止](radar.gif)

打开时从中心展开一次，结束后保持最终形状。[直接查看静态图](radar.svg)。加载与再次打开的播放时机取决于浏览器缓存。

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 刊会质量 | 85.0 | 30% |
| 创新性 | 88 | 20% |
| 实验与证据 | 96 | 20% |
| 学术影响 | 86.9 | 10% |
| 近期关注 | 99.9 | 5% |
| 复用价值 | 99 | 8% |
| 阅读价值 | 97 | 7% |

刊会依据：[TMLR 2024](../../../venues/TMLR/README.md)，正式出处见[出版/原文记录](https://openreview.net/forum?id=a68SUt6zFt)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：DINOv2: Learning Robust Visual Features without Supervision。累计被引 1054，2025–2026 被引 496；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4366208220) · [文献计量条目](https://openalex.org/W4366208220)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
