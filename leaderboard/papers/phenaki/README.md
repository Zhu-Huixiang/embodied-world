# Phenaki: Variable Length Video Generation From Open Domain Textual Descriptions

**Phenaki** · ICLR 2023 · 本版排名 73 · 综合分 **83.2 / 100**

[解读导读](../../../library/phenaki.md) · [视频与序列生成](../../../paper-map/README.md#track-video-generation) · [ICLR集锦](../../../venues/ICLR/README.md)

[原文](https://openreview.net/forum?id=vOEXS39nOF) · [PDF](https://openreview.net/pdf?id=vOEXS39nOF) · [阅读卡片](../../../library/phenaki.md)

## 机制简析

C-ViViT 用因果时间注意力把可变长度视频压成离散 token，兼顾空间与时间压缩。文本特征条件化双向掩码 Transformer，逐轮补齐视频 token 后再解码；继续生成时复用已有上下文。原文检查视频压缩、时序质量和图文/视频联合训练，并展示随文本故事变化的长视频。

带着这个问题读：一段视频怎样变成短 token 序列，因果编码又怎样允许它继续往后生成？

初读判断：可变时长编码与离散生成链路具体，对照能回答 token 预算和时序一致性；公开代码/权重覆盖不如完全开源项目，复用分相应较低。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 89 | 20% |
| 实验与证据 | 87 | 20% |
| 学术影响 | 54.7 | 10% |
| 近期关注 | 33.4 | 5% |
| 复用价值 | 75 | 8% |
| 阅读价值 | 91 | 7% |

刊会依据：[ICLR 2023](../../../venues/ICLR/README.md)，正式出处见[出版/原文记录](https://openreview.net/forum?id=vOEXS39nOF)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：Phenaki: Variable Length Video Generation From Open Domain Textual Description。累计被引 79，2025–2026 被引 7；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4303441850) · [文献计量条目](https://openalex.org/W4303441850)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
