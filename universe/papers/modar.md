# ModAR 星系

Modality-Autoregressive World-Action Models

**导读** · 世界动作模型

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/modar.md) · [原文](https://arxiv.org/abs/2609.17524v1) · [评分卡](../../leaderboard/papers/modar/README.md)

共享DiT把当前DINO/深度/RGB和配置/任务条件融合，按点轨迹→DINO→深度→RGB块自回归去噪，动作最后生成；上下文加噪避免前一模态误差层层放大。实机去掉收益最小的未来RGB。

## 技术挂点

- [世界动作联合建模](../concepts/wam.md)：把未来状态或视频与动作放进联合条件生成过程，让视觉动态和行动相互约束。

- [Diffusion Transformer](../concepts/dit.md)：用 Transformer 实现扩散模型的去噪网络，使 token 之间交换条件与目标信息。

- [因果序列建模](../concepts/causal.md)：通过遮罩只让位置读取允许的历史，避免训练时看到运行时不存在的未来。

## 本篇行星与卫星

- [世界动作联合建模](modar/wam.md) · 初读挂点
- [Diffusion Transformer](modar/dit.md) · 初读挂点
- [因果序列建模](modar/causal.md) · 初读挂点
- [本篇方法链路](modar/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
