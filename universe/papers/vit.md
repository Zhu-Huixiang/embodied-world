# ViT 星系

An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale

**导读** · 具身感知与场景表示

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/vit.md) · [原文](https://iclr.cc/virtual/2021/poster/3013) · [评分卡](../../leaderboard/papers/vit/README.md)

将图像切成固定大小的 patch，每块展平后线性投影为 token，再加入位置编码送进标准 Transformer。原文以大规模监督预训练和小规模下游微调测试数据规模与视觉归纳偏置的关系。实验覆盖 ImageNet、CIFAR 和 VTAB，机器人中的视觉 backbone 是这条表示路线的后续应用。

## 技术挂点

- [视觉 patch token](../concepts/patches.md)：把图像切成块，展平并投影成向量，再加入位置信息。

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。

## 本篇行星与卫星

- [视觉 patch token](vit/patches.md) · 初读挂点
- [注意力](vit/attention.md) · 初读挂点
- [表征空间](vit/representation.md) · 初读挂点
- [本篇方法链路](vit/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
