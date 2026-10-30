# 零末端SNR下的一步DDIM · TAPESTRY

特定日程和v预测使完全噪声端点的目标变为负的干净动作token。

末端alpha_bar=0，xT=epsilon，预测x0=-v_theta(epsilon,T,c)；只一次前向，16动作token输出动作块，不调用未来视频生成和VAE解码。

继续拆：[多步去噪为何越修越抖](jitter.md) · [一步条件均值的多模态代价](conditional-mean.md) · [少token、少前向和小骨干的共同成本收益](cost.md)。

[本篇星系](../tapestry.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/tapestry.md) · [原文依据](https://arxiv.org/pdf/2610.36823v1)
