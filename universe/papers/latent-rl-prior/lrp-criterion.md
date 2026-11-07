# 对齐成功不是十步连续达标 · Latent RL Prior

四个物体与目标对应关键点的最大距离决定姿态对齐是否满足阈值。

d_max=max_j||k_obj_j−k_goal_j||；累计10个policy step达标即可，可不连续；严格0.015m、宽松0.05m两套结果分开。

[本篇星系](../latent-rl-prior.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/latent-rl-prior.md) · [原文依据](https://arxiv.org/pdf/2611.08458v1)
