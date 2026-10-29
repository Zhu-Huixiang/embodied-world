# ViT 星系

An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale

**已精讲** · 具身感知与场景表示

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/vit-2010.11929/README.md) · [原文](https://iclr.cc/virtual/2021/poster/3013) · [评分卡](../../leaderboard/papers/vit/README.md)

将图像切成固定大小的 patch，每块展平后线性投影为 token，再加入位置编码送进标准 Transformer。原文以大规模监督预训练和小规模下游微调测试数据规模与视觉归纳偏置的关系。实验覆盖 ImageNet、CIFAR 和 VTAB，机器人中的视觉 backbone 是这条表示路线的后续应用。

## 技术挂点

- [视觉 patch token](../concepts/patches.md)：把图像切成块，展平并投影成向量，再加入位置信息。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/vit-2010.11929/README.md#31-a-区切块不是把信息扔掉是先换个包装)

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/vit-2010.11929/README.md#31-b-区注意力不是看见重点的黑箱)

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/vit-2010.11929/README.md#31-cd-区cls-的代表发言权怎么来的)

- [线性探测](../concepts/linear-probe.md)：冻结编码器，用带标签的下游样本训练线性预测头，以检查特征本身是否容易迁移。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/vit-2010.11929/README.md#43-数据需求大模型吃瘪那张图才是论文的转折)

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/vit-2010.11929/README.md#45-检查内部位置表有没有学出附近)

## 本篇行星与卫星

- [视觉 patch token](vit/patches.md) · 已讲解
- [注意力](vit/attention.md) · 已讲解
- [表征空间](vit/representation.md) · 已讲解
- [线性探测](vit/linear-probe.md) · 已讲解
- [空间表示](vit/spatial.md) · 已讲解
- [本篇方法链路](vit/method-chain.md) · 已讲解
- [切块与线性投影](vit/patch-projection.md) · 已讲解
- [位置编码与二维插值](vit/position.md) · 已讲解
- [Pre-LN与残差](vit/pre-ln.md) · 已讲解
- [QKV与多头注意力](vit/qkv.md) · 已讲解
- [CLS读出与分类头](vit/cls.md) · 已讲解
- [数据规模与结构先验](vit/data-scale.md) · 已讲解
- [算力与分辨率](vit/compute.md) · 已讲解
- [空间结构的事后观察](vit/spatial-probe.md) · 已讲解
- [早期掩码块预测](vit/mpp.md) · 已讲解

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
