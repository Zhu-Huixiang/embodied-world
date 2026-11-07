# 视觉小步更新，动作先验保持冻结 · Latent RL Prior

分别扫描image encoder与action decoder学习率，Q-Former始终训练。

Fig7a固定decoder、小视觉学习率有利严格对齐，大更新尤其低数据退化；Fig7b固定image encoder，decoder解冻在所测范围无益。两扫描条件不可误合成同一次全参数实验。

[本篇星系](../latent-rl-prior.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/latent-rl-prior.md) · [原文依据](https://arxiv.org/pdf/2611.08458v1)
