# DINOv2: Learning Robust Visual Features without Supervision

**解读导读** · TMLR 2024 · [具身感知与场景表示](../paper-map/README.md#track-embodied-perception)

研究范围：生成/表征基础，OpenVLA 实际采用的 DINOv2 视觉编码器。

[原文入口](https://openreview.net/forum?id=a68SUt6zFt) · [原文 PDF](https://openreview.net/pdf?id=a68SUt6zFt) · [作者项目 / 代码入口](https://github.com/facebookresearch/dinov2) · [作者与团队](../leaderboard/origins/papers/dinov2.md)

TMLR 2024-01 正式论文，arXiv 初始公开于 2023；作者 HAL 存档 PDF 首页明确写 Published in Transactions on Machine Learning Research (01/2024)。OpenReview forum 抓取受验证页影响，PDF 与作者存档可读。

## 先看它做了什么

在大规模筛选图像上扩展图像级与 patch 级自监督学习，再把大 ViT 教师蒸馏为不同尺寸的编码器。下游可以冻结 backbone，用轻量预测头读取分类、分割或深度相关信息。原文比较多种图像与像素任务；OpenVLA 的视觉输入实际将 DINOv2 特征与 SigLIP 特征拼接后映射给语言模型。

## 带着什么问题读

**机器人视觉编码器冻结以后，哪些几何和语义信息还能留在 patch 特征里？**

## 为什么值得继续读

OpenVLA 正式原文明确融合 DINOv2 与 SigLIP 特征，具身用途已由下游原文核实；数据筛选和冻结特征迁移值得精讲。

证据入口：广泛冻结特征评估、数据与规模设计及开放权重形成很强复用价值；与机器人策略的连接由 OpenVLA 原文确认。

具身关联：OpenVLA 正式原文明确融合 DINOv2 与 SigLIP 特征，具身用途已由下游原文核实；数据筛选和冻结特征迁移值得精讲。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/dinov2/README.md) · [TMLR集锦](../venues/TMLR/README.md) · [地图方向](../paper-map/README.md#track-embodied-perception) · [首页](../README.md)

元数据核对：2026-10-10。
