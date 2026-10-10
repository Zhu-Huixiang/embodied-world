# Phenaki: Variable Length Video Generation From Open Domain Textual Descriptions

**解读导读** · ICLR 2023 · [视频与序列生成](../paper-map/README.md#track-video-generation)

研究范围：生成/表征基础，因果视频 token、长序列生成与视频动作建模的离散路线。

[原文入口](https://openreview.net/forum?id=vOEXS39nOF) · [原文 PDF](https://openreview.net/pdf?id=vOEXS39nOF) · [作者项目 / 代码入口](https://sites.research.google/gr/phenaki/) · [作者与团队](../leaderboard/origins/papers/phenaki.md)

ICLR 2023 正式论文，官方 PDF 首页确认；主要是文本到视频生成基础。

## 先看它做了什么

C-ViViT 用因果时间注意力把可变长度视频压成离散 token，兼顾空间与时间压缩。文本特征条件化双向掩码 Transformer，逐轮补齐视频 token 后再解码；继续生成时复用已有上下文。原文检查视频压缩、时序质量和图文/视频联合训练，并展示随文本故事变化的长视频。

## 带着什么问题读

**一段视频怎样变成短 token 序列，因果编码又怎样允许它继续往后生成？**

## 为什么值得继续读

因果视频 tokenizer、掩码 Transformer 和混合图文/视频训练给出完整离散视频路线，可与扩散世界模型形成有机制的对照。

证据入口：可变时长编码与离散生成链路具体，对照能回答 token 预算和时序一致性；公开代码/权重覆盖不如完全开源项目，复用分相应较低。

具身关联：因果视频 tokenizer、掩码 Transformer 和混合图文/视频训练给出完整离散视频路线，可与扩散世界模型形成有机制的对照。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/phenaki/README.md) · [ICLR集锦](../venues/ICLR/README.md) · [地图方向](../paper-map/README.md#track-video-generation) · [首页](../README.md)

元数据核对：2026-10-10。
