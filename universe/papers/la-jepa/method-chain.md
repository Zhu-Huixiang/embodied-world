# 本篇方法链路 · La-JEPA

La-JEPA以预训练V-JEPA 2.1 ViT-L编码当前两帧和32帧范围内的未来16帧，FLAN-T5-large编码语言，本体投影为条件token。在该表征空间从头训练World DiT和Action DiT，分别对未来特征与32步动作块做独立时间的流匹配。观测只读观测、未来读观测和未来、动作只读观测和动作；未来损失通过共享World参数影响观测表示。部署删除未来token，固定World时间0并缓存观测K/V，仅对动作做10步Euler积分，LIBERO执行10步、RoboTwin执行24步后重规划。最终观测编码器用LoRA和增强，未来目标保持原冻结编码器的干净特征；无需像素解码。

La-JEPA以预训练V-JEPA 2.1 ViT-L编码当前两帧和32帧范围内的未来16帧，FLAN-T5-large编码语言，本体投影为条件token。在该表征空间从头训练World DiT和Action DiT，分别对未来特征与32步动作块做独立时间的流匹配。观测只读观测、未来读观测和未来、动作只读观测和动作；未来损失通过共享World参数影响观测表示。部署删除未来token，固定World时间0并缓存观测K/V，仅对动作做10步Euler积分，LIBERO执行10步、RoboTwin执行24步后重规划。最终观测编码器用LoRA和增强，未来目标保持原冻结编码器的干净特征；无需像素解码。

[本篇星系](../la-jepa.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/la-jepa.md) · [原文依据](https://arxiv.org/abs/2611.08156v1)
