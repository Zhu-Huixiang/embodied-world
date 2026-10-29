# DiT 星系

Scalable Diffusion Models with Transformers

**已精讲** · Diffusion / Transformer 基础

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dit-2212.09748/README.md) · [原文](https://openaccess.thecvf.com/content/ICCV2023/html/Peebles_Scalable_Diffusion_Models_with_Transformers_ICCV_2023_paper.html) · [评分卡](../../leaderboard/papers/dit/README.md)

在图像潜表示的patch序列上用Transformer做扩散去噪，考察计算规模和条件注入。

## 技术挂点

- [Diffusion Transformer](../concepts/dit.md)：用 Transformer 实现扩散模型的去噪网络，使 token 之间交换条件与目标信息。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dit-2212.09748/README.md#3-diffusion-transformers拆开-abc)

- [视觉 patch token](../concepts/patches.md)：把图像切成块，展平并投影成向量，再加入位置信息。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dit-2212.09748/README.md#32-设计空间patchify-怎么切)

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dit-2212.09748/README.md#block-内部token-之间怎样互相看)

- [扩散去噪](../concepts/diffusion.md)：训练网络从带噪对象估计噪声或干净目标，生成时从噪声开始迭代恢复样本。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dit-2212.09748/README.md#31-先交代潜变量和噪声)

- [条件生成](../concepts/generation.md)：从一个条件生成多个可能输出，学习图像、视频或动作的分布而非只给一个均值。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dit-2212.09748/README.md#6-结论三个问题分别落地)

## 本篇行星与卫星

- [Diffusion Transformer](dit/dit.md) · 已讲解
- [视觉 patch token](dit/patches.md) · 已讲解
- [注意力](dit/attention.md) · 已讲解
- [扩散去噪](dit/diffusion.md) · 已讲解
- [条件生成](dit/generation.md) · 已讲解
- [本篇方法链路](dit/method-chain.md) · 初读挂点
- [潜变量切块](dit/patch.md) · 已讲解
- [多头自注意力](dit/attn.md) · 已讲解
- [条件调制与残差门](dit/adaln.md) · 已讲解
- [噪声和协方差输出](dit/output.md) · 已讲解
- [类别无分类器引导](dit/cfg.md) · 已讲解
- [模型与token双扩展](dit/scaling.md) · 已讲解
- [主干质量与采样计算](dit/sampling.md) · 已讲解

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
