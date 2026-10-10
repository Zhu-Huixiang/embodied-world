# Where are we in the search for an Artificial Visual Cortex for Embodied Intelligence?

**解读导读** · NeurIPS 2023 · [具身感知与场景表示](../paper-map/README.md#track-embodied-perception)

研究范围：VC-1、CortexBench 与跨具身任务视觉预训练评测。

[原文入口](https://proceedings.neurips.cc/paper_files/paper/2023/hash/022ca1bed6b574b962c48a2856eb207b-Abstract-Conference.html) · [原文 PDF](https://proceedings.neurips.cc/paper_files/paper/2023/file/022ca1bed6b574b962c48a2856eb207b-Paper-Conference.pdf) · [作者项目 / 代码入口](https://eai-vc.github.io/) · [作者与团队](../leaderboard/origins/papers/vc1.md)

NeurIPS 2023 正式版。项目与论文数据图像总量可能不同，精读使用固定正式版；平均优势与逐任务优势分开。

## 先看它做了什么

先把导航、移动操作、灵巧操作和运动控制纳入 CortexBench，统一比较不同预训练视觉模型。固定 MAE 目标后变化视频来源、数据规模和 ViT 容量，再检验同一编码器能否处处占优。VC-1 的平均提升和任务适配提升分别报告，暴露视觉预训练的任务差异。

## 带着什么问题读

**有没有一套视觉编码器在所有具身任务上都强？扩大人类视频数据就够了吗？**

## 为什么值得继续读

对具身视觉基础模型进行广覆盖系统检验的重要工作，避免只靠单一操作基准宣称通用感知。

证据入口：NeurIPS 正式版明确是系统评估而非新算法，跨领域任务、数据/容量研究、硬件实验和公开模型构成强证据；榜单应奖励研究设计而非包装新模块。

具身关联：对具身视觉基础模型进行广覆盖系统检验的重要工作，避免只靠单一操作基准宣称通用感知。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/vc1/README.md) · [NeurIPS集锦](../venues/NeurIPS/README.md) · [地图方向](../paper-map/README.md#track-embodied-perception) · [首页](../README.md)

元数据核对：2026-10-10。
