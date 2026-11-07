# 动作先验学的是条件速度场 · Latent RL Prior

干净动作A0与高斯噪声A1线性插值，网络拟合A1−A0。

Aτ=(1−τ)A0+τA1，τ均匀于[0,1]；训练MSE为||vθ(Aτ,τ,Z,R)−(A1−A0)||²。A0是数据、A1是噪声，生成方向应从τ=1回到0；本文未列推理步数。

[本篇星系](../latent-rl-prior.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/latent-rl-prior.md) · [原文依据](https://arxiv.org/pdf/2611.08458v1)
