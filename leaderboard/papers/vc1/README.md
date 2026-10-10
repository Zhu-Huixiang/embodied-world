# Where are we in the search for an Artificial Visual Cortex for Embodied Intelligence?

本版阅读优先顺序：63；综合分：84.1 / 100；已评分权重：100%。

[原文](https://proceedings.neurips.cc/paper_files/paper/2023/hash/022ca1bed6b574b962c48a2856eb207b-Abstract-Conference.html) · [PDF](https://proceedings.neurips.cc/paper_files/paper/2023/file/022ca1bed6b574b962c48a2856eb207b-Paper-Conference.pdf) · [阅读卡片](../../../library/vc1.md)

## 机制简析

先把导航、移动操作、灵巧操作和运动控制纳入 CortexBench，统一比较不同预训练视觉模型。固定 MAE 目标后变化视频来源、数据规模和 ViT 容量，再检验同一编码器能否处处占优。VC-1 的平均提升和任务适配提升分别报告，暴露视觉预训练的任务差异。

带着这个问题读：有没有一套视觉编码器在所有具身任务上都强？扩大人类视频数据就够了吗？

初读判断：NeurIPS 正式版明确是系统评估而非新算法，跨领域任务、数据/容量研究、硬件实验和公开模型构成强证据；榜单应奖励研究设计而非包装新模块。

## 七维评分

![七维雷达：加载时展开一次，随后静止](radar.gif)

打开时从中心展开一次，结束后保持最终形状。[直接查看静态图](radar.svg)。加载与再次打开的播放时机取决于浏览器缓存。

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 刊会质量 | 95.0 | 30% |
| 创新性 | 84 | 20% |
| 实验与证据 | 95 | 20% |
| 学术影响 | 38.6 | 10% |
| 近期关注 | 28.8 | 5% |
| 复用价值 | 98 | 8% |
| 阅读价值 | 95 | 7% |

刊会依据：[NeurIPS 2023](../../../venues/NeurIPS/README.md)，正式出处见[出版/原文记录](https://proceedings.neurips.cc/paper_files/paper/2023/hash/022ca1bed6b574b962c48a2856eb207b-Abstract-Conference.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：Where are we in the search for an Artificial Visual Cortex for Embodied Intelligence?。累计被引 21，2025–2026 被引 5；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4362514550) · [文献计量条目](https://openalex.org/W4362514550)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
