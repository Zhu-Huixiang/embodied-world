# 直接预测latent，不先猜物理状态 · Latent RL Prior

latent transfer把图像特征直接变为动作decoder可消费的context。

Z_latent=Q_ϕ(E_vis(I_t))，替换原state tokenizer和state Q-Former；只需动作流匹配loss。context无需可解释成物体位姿。

继续拆：[两组queries协调，同一decoder分别出动作](lrp-bimanual.md) · [固定视觉特征后仍有先验收益](lrp-scratch.md)。

[本篇星系](../latent-rl-prior.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/latent-rl-prior.md) · [原文依据](https://arxiv.org/pdf/2611.08458v1)
