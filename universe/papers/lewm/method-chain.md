# 本篇方法链路 · LeWM

ViT将每帧变成192维CLS表征；动作AdaLN条件的Transformer预测下个latent。MSE预测+SIGReg随机投影高斯正则共同训练，无EMA/stop-gradient/重建。部署用latent目标距离和CEM选动作，再MPC重规划。

ViT将每帧变成192维CLS表征；动作AdaLN条件的Transformer预测下个latent。MSE预测+SIGReg随机投影高斯正则共同训练，无EMA/stop-gradient/重建。部署用latent目标距离和CEM选动作，再MPC重规划。

[本篇星系](../lewm.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/lewm.md) · [原文依据](https://arxiv.org/abs/2603.19312v1)
