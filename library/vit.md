# An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale

出处：ICLR 2021。研究范围：生成/表征基础，机器人视觉编码器与 VLA 图像 token 的入口。

[原文入口](https://iclr.cc/virtual/2021/poster/3013) · [原文 PDF](https://arxiv.org/pdf/2010.11929v2) · [作者项目 / 代码入口](https://github.com/google-research/vision_transformer)

ICLR 2021 正式论文；此条对应原始 ViT，不将后来的自监督或机器人结果算作本篇实验。

阅读问题：**一张图怎样变成 token 序列，机器人策略拿到的视觉特征来自哪一步？**

收录理由：ViT 的图像 patch 序列成为 DINOv2、MAE 及多种 VLA 视觉编码器的共同架构；MVP 原文直接采用 ViT 做实机视觉预训练。

证据入口：架构变化直接，数据规模与 CNN 对照有解释力，权重与微调实现公开；先读能减少后续 VLA 编码器的理解负担。

具身关联：ViT 的图像 patch 序列成为 DINOv2、MAE 及多种 VLA 视觉编码器的共同架构；MVP 原文直接采用 ViT 做实机视觉预训练。

经典保留理由：ICLR 2021 早于 2021-10-10，作为图像 token 化的经典例外；后续机器人视觉预训练和 VLA 明确采用其结构。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/vit/README.md)

机制简析：将图像切成固定大小的 patch，每块展平后线性投影为 token，再加入位置编码送进标准 Transformer。原文以大规模监督预训练和小规模下游微调测试数据规模与视觉归纳偏置的关系。实验覆盖 ImageNet、CIFAR 和 VTAB，机器人中的视觉 backbone 是这条表示路线的后续应用。
<!-- discovery:end -->
