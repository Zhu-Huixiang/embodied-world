# SAM 星系

Segment Anything

**已精讲** · 具身感知与场景表示

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam-2304.02643/README.md) · [原文](https://openaccess.thecvf.com/content/ICCV2023/html/Kirillov_Segment_Anything_ICCV_2023_paper.html) · [评分卡](../../leaderboard/papers/sam/README.md)

图像编码器先算一次图像特征，点、框或已有掩码由提示编码器表达，轻量掩码解码器联合两者预测目标区域。一次图像编码可以服务多次交互，模型同时输出多个候选以应对提示歧义。数据引擎让模型辅助人工标注再改进模型，原文以零样本图像分割和不同提示任务验证迁移。

## 技术挂点

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam-2304.02643/README.md#31-a-区大图压成一张可反复查询的特征地图)

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam-2304.02643/README.md#33-c-区提示看图图也回头看提示)

- [零样本任务接口](../concepts/zero-shot.md)：不用目标数据集训练样本拟合分类头，而用任务描述等已有信息直接构造预测接口。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam-2304.02643/README.md#61-先看单点再看多点)

- [视觉 patch token](../concepts/patches.md)：把图像切成块，展平并投影成向量，再加入位置信息。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam-2304.02643/README.md#31-a-区大图压成一张可反复查询的特征地图)

## 本篇行星与卫星

- [空间表示](sam/spatial.md) · 已讲解
- [注意力](sam/attention.md) · 已讲解
- [零样本任务接口](sam/zero-shot.md) · 已讲解
- [视觉 patch token](sam/patches.md) · 已讲解
- [本篇方法链路](sam/method-chain.md) · 初读挂点
- [可提示分割](sam/task.md) · 已讲解
- [单点歧义](sam/ambiguity.md) · 已讲解
- [可缓存图像编码](sam/cache.md) · 已讲解
- [视觉块与空间网格](sam/patch.md) · 已讲解
- [MAE预训练](sam/mae.md) · 已讲解
- [点框提示编码](sam/sparse.md) · 已讲解
- [密集掩码提示](sam/dense.md) · 已讲解
- [双向注意力解码](sam/decoder.md) · 已讲解
- [交叉注意力的两种方向](sam/cross.md) · 已讲解
- [掩码超网络读出](sam/readout.md) · 已讲解
- [多候选最小损失](sam/min-loss.md) · 已讲解
- [IoU与质量预测](sam/iou.md) · 已讲解
- [模拟交互训练](sam/interactive-train.md) · 已讲解
- [三阶段数据引擎](sam/engine.md) · 已讲解
- [自动掩码过滤](sam/filter.md) · 已讲解
- [数据覆盖与责任分析](sam/distribution.md) · 已讲解
- [零样本分割评测](sam/zero-transfer.md) · 已讲解
- [检测与分割分工](sam/detector-box.md) · 已讲解
- [文本提示概念变体](sam/text-variant.md) · 已讲解
- [数据与模型规模消融](sam/scaling.md) · 已讲解

## 论文间的联系

- [SAM](sam.md) → [Transformer](attention.md)：SAM的图像骨干与双向解码器使用Transformer注意力模块；本文在3.1–3.3拆解两路交互。 [原文定位](https://arxiv.org/abs/2304.02643v1)（§3; Appendix A）。

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
