# 显式桥接也只有动作监督 · Latent RL Prior

explicit transfer先预测具有特权状态形状的历史，再走冻结state encoder。

P_hat=B_ρ(E_vis(I_t))，Z_explicit=Q_ψ(T_η(P_hat))；T_η、Q_ψ、vθ全部冻结，只训练图像编码器和桥。该对照未使用真实特权标签监督预测状态。

继续拆：[latent接口比显式形状桥更稳](lrp-interface-ablation.md)。

[本篇星系](../latent-rl-prior.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/latent-rl-prior.md) · [原文依据](https://arxiv.org/pdf/2611.08458v1)
