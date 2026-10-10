# Masked Autoencoders Are Scalable Vision Learners

**解读导读** · CVPR 2022 · [具身感知与场景表示](../paper-map/README.md#track-embodied-perception)

研究范围：生成/表征基础，MVP 等机器人视觉预训练的掩码重建算法。

[原文入口](https://openaccess.thecvf.com/content/CVPR2022/html/He_Masked_Autoencoders_Are_Scalable_Vision_Learners_CVPR_2022_paper.html) · [原文 PDF](https://openaccess.thecvf.com/content/CVPR2022/papers/He_Masked_Autoencoders_Are_Scalable_Vision_Learners_CVPR_2022_paper.pdf) · [作者项目 / 代码入口](https://github.com/facebookresearch/mae) · [作者与团队](../leaderboard/origins/papers/mae.md)

CVPR 2022 正式论文；与机器人实机扩展 MVP 分开记录，后者是 CoRL 2022、论文集 2023。

## 先看它做了什么

随机遮住大部分图像 patch，编码器只处理可见部分，轻量解码器再接入 mask token 还原缺失像素。非对称结构减少昂贵编码器的计算，高遮挡比例让补全任务需要理解物体和场景。原文比较分类、检测、分割迁移；MVP 将同类编码器冻结后接到可训练控制模块。

## 带着什么问题读

**遮住四分之三的图像后还原像素，怎样帮助机器人把预训练视觉特征用于控制？**

## 为什么值得继续读

MVP 原文直接用 MAE 预训练视觉表示并在多种实机任务中检验，关联不是泛泛的潜在用途。

证据入口：方法和计算节省能直接从结构理解，视觉迁移实验完整，官方实现公开；机器人实机继承关系有 MVP 原文佐证。

具身关联：MVP 原文直接用 MAE 预训练视觉表示并在多种实机任务中检验，关联不是泛泛的潜在用途。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/mae/README.md) · [CVPR集锦](../venues/CVPR/README.md) · [地图方向](../paper-map/README.md#track-embodied-perception) · [首页](../README.md)

元数据核对：2026-10-10。
