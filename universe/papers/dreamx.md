# DreamX 星系

DreamX: Video Diffusion Model is a Universal Latent Action Learner

**导读** · 视频动作模型与视觉推理

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamx.md) · [原文](https://arxiv.org/abs/2611.05377v1) · [评分卡](../../leaderboard/papers/dreamx/README.md)

DreamX用Cosmos-Predict2.5 2B的时空特征直接读出动作latent：每个VAE潜帧分配4个可学习query，最长32个2048维token。编码与解码分别用rank16 LoRA，骨干冻结；解码器从首帧和query重建未来，有机器人标签时另加动作流匹配损失，视频流与动作流不互相注意。预训练混合约2.19k小时人/机器人视频。一个变分瓶颈再把每token压到32维；下游策略由当前画面和文字预测这些code，动作DiT读取latent特征和本体状态，不在控制时生成未来视频。源视频迁移则冻结编码器/解码器，换目标首帧生成视频，或换目标初始状态解码开放环动作。

## 技术挂点

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。

- [Flow Matching](../concepts/flow.md)：给噪声到数据指定概率路径，回归沿路径的速度场；生成时数值积分这个场。

- [Diffusion Transformer](../concepts/dit.md)：用 Transformer 实现扩散模型的去噪网络，使 token 之间交换条件与目标信息。

- [变分自编码器 VAE](../concepts/vae.md)：编码器描述潜变量分布，解码器从潜变量重建样本，用重建与分布正则共同训练。

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

- [机器人数据与评测](../concepts/data.md)：统一观测、动作、任务与评测条件，判断数据多样性如何影响泛化。

- [跨本体数据](../concepts/cross-body.md)：从多个机器人或人类收集经验，通过动作/观测适配接到共享学习系统。

- [视频时序生成](../concepts/video.md)：同时表达画面内容与时间变化，用历史与条件产生连续帧。

## 本篇行星与卫星

- [表征空间](dreamx/representation.md) · 初读挂点
- [注意力](dreamx/attention.md) · 初读挂点
- [Flow Matching](dreamx/flow.md) · 初读挂点
- [Diffusion Transformer](dreamx/dit.md) · 初读挂点
- [变分自编码器 VAE](dreamx/vae.md) · 初读挂点
- [动作表示](dreamx/action.md) · 初读挂点
- [机器人数据与评测](dreamx/data.md) · 初读挂点
- [跨本体数据](dreamx/cross-body.md) · 初读挂点
- [视频时序生成](dreamx/video.md) · 初读挂点
- [本篇方法链路](dreamx/method-chain.md) · 初读挂点
- [从视频重建到可迁移动作](dreamx/dx-problem.md) · 初读挂点
- [同一视频先验的编码与解码角色](dreamx/dx-backbone.md) · 初读挂点
- [5到29帧怎样变成潜视频](dreamx/dx-video-latents.md) · 初读挂点
- [每个潜帧只读出四个查询](dreamx/dx-queries.md) · 初读挂点
- [直接历史读取不等于全网因果](dreamx/dx-encoder-mask.md) · 初读挂点
- [编码用文字，重建用latent](dreamx/dx-language.md) · 初读挂点
- [视频与动作共用条件而不互读](dreamx/dx-decoder-mask.md) · 初读挂点
- [有动作标签才加入动作损失](dreamx/dx-loss.md) · 初读挂点
- [2190小时不是全为人类视频](dreamx/dx-data.md) · 初读挂点
- [同一latent换一个起始画面](dreamx/dx-video-transfer.md) · 初读挂点
- [从人类动作到开放环机器轨迹](dreamx/dx-action-transfer.md) · 初读挂点
- [32乘2048再压成32乘32](dreamx/dx-bottleneck.md) · 初读挂点
- [控制时预测code而非生成未来视频](dreamx/dx-policy.md) · 初读挂点
- [预训练与任务微调两笔成本](dreamx/dx-policy-training.md) · 初读挂点
- [公共probe测表示，不是闭环成功率](dreamx/dx-lary-protocol.md) · 初读挂点
- [表征误差与语义分类同时改善](dreamx/dx-lary-results.md) · 初读挂点
- [1008段视频如何做零样本迁移评估](dreamx/dx-hr-protocol.md) · 初读挂点
- [视频迁移保运动也保目标外观](dreamx/dx-hr-results.md) · 初读挂点
- [双臂YAM的14维绝对动作](dreamx/dx-real-setup.md) · 初读挂点
- [96.7%是两个子目标的平均](dreamx/dx-real-metric.md) · 初读挂点
- [小latent减少生成对象，但仍有推理成本](dreamx/dx-latency.md) · 初读挂点
- [上抽屉人类监督仍有其他机器人数据](dreamx/dx-human-only.md) · 初读挂点
- [动作标签对表征的贡献很小且非单向](dreamx/dx-action-ablation.md) · 初读挂点
- [latent条件是否真被动作头用到](dreamx/dx-policy-ablation.md) · 初读挂点
- [扰动latent首先改变运动](dreamx/dx-perturbation.md) · 初读挂点
- [方向簇是聚合均值而非逐样本解耦](dreamx/dx-centroids.md) · 初读挂点
- [表示迁移、生成迁移与闭环策略三层证据](dreamx/dx-scope.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
