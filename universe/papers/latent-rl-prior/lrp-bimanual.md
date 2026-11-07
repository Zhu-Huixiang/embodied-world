# 两组queries协调，同一decoder分别出动作 · Latent RL Prior

左右臂各M个query先共同经视觉Q-Former自注意力交互。

左右Z再分别和各臂本体历史送入同权重冻结单臂decoder；协调发生于context，不是把双臂状态拼进一个新decoder。

[本篇星系](../latent-rl-prior.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/latent-rl-prior.md) · [原文依据](https://arxiv.org/pdf/2611.08458v1)
