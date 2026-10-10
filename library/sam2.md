# SAM 2: Segment Anything in Images and Videos

**解读导读** · ICLR 2025 · [具身感知与场景表示](../paper-map/README.md#track-embodied-perception)

研究范围：生成/表征基础，机器人视频中的目标跟踪与时序分割。

[原文入口](https://openreview.net/forum?id=Ha6RTeWMd0) · [原文 PDF](https://proceedings.iclr.cc/paper_files/paper/2025/file/45c1f6a8cbf2da59ebf2c802b4f742cd-Paper-Conference.pdf) · [作者项目 / 代码入口](https://github.com/facebookresearch/sam2)

ICLR 2025 正式论文，首次预印本 2024；官方 PDF 首页确认 ICLR 2025。

## 先看它做了什么

逐帧图像特征通过记忆注意力读取之前的目标提示与掩码信息，再与当前提示一起预测本帧掩码。记忆编码器把当前预测存入记忆，下一帧继续使用；静态图像相当于记忆为空的视频。原文比较交互次数、速度以及图像和视频分割基准。

## 带着什么问题读

**目标在机器人视野里移动、遮挡后重现，过去的掩码记忆怎样帮它跟住对象？**

## 为什么值得继续读

SAM 2 原文直接讨论机器人时序定位需求，流式记忆把静态提示分割扩展到视频；正式评测含多种视频与图像分布。

证据入口：流式记忆和对象持续性问题直接，跨数据集与交互成本评估较完整，代码、模型及视频分割数据公开。

具身关联：SAM 2 原文直接讨论机器人时序定位需求，流式记忆把静态提示分割扩展到视频；正式评测含多种视频与图像分布。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/sam2/README.md) · [ICLR集锦](../venues/ICLR/README.md) · [地图方向](../paper-map/README.md#track-embodied-perception) · [首页](../README.md)

元数据核对：2026-10-10。
