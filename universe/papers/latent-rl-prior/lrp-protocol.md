# 比较的是示范预算，不是相同训练预算 · Latent RL Prior

本法100,000优化步，π0.5与GR00T N1.7全参数微调30,000步。

每5,000步存checkpoint，最后5个各测256个保留环境seed rollout；每run取五者最高，通常3训练seed均值±标准差。不是5checkpoint平均，也不是训练算力匹配。

继续拆：[50条抬门、1000条双臂的比较条件](lrp-data-efficiency.md)。

[本篇星系](../latent-rl-prior.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/latent-rl-prior.md) · [原文依据](https://arxiv.org/pdf/2611.08458v1)
