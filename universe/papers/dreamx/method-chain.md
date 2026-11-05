# 本篇方法链路 · DreamX

DreamX用Cosmos-Predict2.5 2B的时空特征直接读出动作latent：每个VAE潜帧分配4个可学习query，最长32个2048维token。编码与解码分别用rank16 LoRA，骨干冻结；解码器从首帧和query重建未来，有机器人标签时另加动作流匹配损失，视频流与动作流不互相注意。预训练混合约2.19k小时人/机器人视频。一个变分瓶颈再把每token压到32维；下游策略由当前画面和文字预测这些code，动作DiT读取latent特征和本体状态，不在控制时生成未来视频。源视频迁移则冻结编码器/解码器，换目标首帧生成视频，或换目标初始状态解码开放环动作。

DreamX用Cosmos-Predict2.5 2B的时空特征直接读出动作latent：每个VAE潜帧分配4个可学习query，最长32个2048维token。编码与解码分别用rank16 LoRA，骨干冻结；解码器从首帧和query重建未来，有机器人标签时另加动作流匹配损失，视频流与动作流不互相注意。预训练混合约2.19k小时人/机器人视频。一个变分瓶颈再把每token压到32维；下游策略由当前画面和文字预测这些code，动作DiT读取latent特征和本体状态，不在控制时生成未来视频。源视频迁移则冻结编码器/解码器，换目标首帧生成视频，或换目标初始状态解码开放环动作。

[本篇星系](../dreamx.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamx.md) · [原文依据](https://arxiv.org/abs/2611.05377v1)
