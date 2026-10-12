# DINOv2 星系

DINOv2: Learning Robust Visual Features without Supervision

**导读** · 具身感知与场景表示

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dinov2.md) · [原文](https://openreview.net/forum?id=a68SUt6zFt) · [评分卡](../../leaderboard/papers/dinov2/README.md)

在大规模筛选图像上扩展图像级与 patch 级自监督学习，再把大 ViT 教师蒸馏为不同尺寸的编码器。下游可以冻结 backbone，用轻量预测头读取分类、分割或深度相关信息。原文比较多种图像与像素任务；OpenVLA 的视觉输入实际将 DINOv2 特征与 SigLIP 特征拼接后映射给语言模型。

## 技术挂点

- [教师学生蒸馏](../concepts/distill.md)：用教师的预测或动作监督学生，让部署模型复制可用行为。

- [视觉 patch token](../concepts/patches.md)：把图像切成块，展平并投影成向量，再加入位置信息。

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。

## 本篇行星与卫星

- [教师学生蒸馏](dinov2/distill.md) · 初读挂点
- [视觉 patch token](dinov2/patches.md) · 初读挂点
- [表征空间](dinov2/representation.md) · 初读挂点
- [本篇方法链路](dinov2/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
