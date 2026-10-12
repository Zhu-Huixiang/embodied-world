# DiT 星系

Scalable Diffusion Models with Transformers

**导读** · Diffusion / Transformer 基础

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dit.md) · [原文](https://openaccess.thecvf.com/content/ICCV2023/html/Peebles_Scalable_Diffusion_Models_with_Transformers_ICCV_2023_paper.html) · [评分卡](../../leaderboard/papers/dit/README.md)

在图像潜表示的patch序列上用Transformer做扩散去噪，考察计算规模和条件注入。

## 技术挂点

- [Diffusion Transformer](../concepts/dit.md)：用 Transformer 实现扩散模型的去噪网络，使 token 之间交换条件与目标信息。

- [视觉 patch token](../concepts/patches.md)：把图像切成块，展平并投影成向量，再加入位置信息。

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。

## 本篇行星与卫星

- [Diffusion Transformer](dit/dit.md) · 初读挂点
- [视觉 patch token](dit/patches.md) · 初读挂点
- [注意力](dit/attention.md) · 初读挂点
- [本篇方法链路](dit/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
