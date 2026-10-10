# 3D Gaussian Splatting for Real-Time Radiance Field Rendering

**解读导读** · SIGGRAPH / TOG 2023 · [具身感知与场景表示](../paper-map/README.md#track-embodied-perception)

研究范围：生成/表征基础，机器人可编辑场景地图与数字场景重建。

[原文入口](https://dl.acm.org/doi/10.1145/3592433) · [原文 PDF](https://arxiv.org/pdf/2308.04079) · [作者项目 / 代码入口](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/)

SIGGRAPH 2023 / ACM TOG 42(4)，ACM 页面给出 2023-07-26；作者项目低清 PDF 含旧模板年份占位，正式年份按 ACM 与项目 BibTeX 核验。

## 先看它做了什么

从相机标定产生的稀疏点初始化三维高斯，优化位置、各向异性形状、不透明度与颜色。可微 splatting 渲染器把高斯投到图像平面，按可见性排序混合；训练中交替优化参数和增删高斯。原文比较多套真实场景的新视角质量、训练时间和渲染速度，后续机器人系统利用同类表示做语义掩码与场景编辑。

## 带着什么问题读

**把神经场换成一群可编辑高斯，为什么渲染会快，场景操作又会方便在哪里？**

## 为什么值得继续读

Splat-MOVER 正式 CoRL 2024 原文直接把可编辑 Gaussian Splatting 用于多阶段机器人操作；原始表示论文贡献和应用结果分开。

证据入口：显式表示与高效渲染共同改变场景构建成本，标准场景对照充分，参考实现公开；CoRL 应用提供直接具身联系。

具身关联：Splat-MOVER 正式 CoRL 2024 原文直接把可编辑 Gaussian Splatting 用于多阶段机器人操作；原始表示论文贡献和应用结果分开。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/gaussian-splatting/README.md) · [SIGGRAPH / TOG集锦](../venues/SIGGRAPH-TOG/README.md) · [地图方向](../paper-map/README.md#track-embodied-perception) · [首页](../README.md)

元数据核对：2026-10-10。
