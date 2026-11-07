# 特权历史先变为任务context · Latent RL Prior

state tokenizer和state Q-Former将物体/目标历史映射为Z_priv。

Z_priv=Q_ψ(T_η(P_t))；动作token交叉注意力读context，本体历史与flow time通过每层AdaLN送入。

继续拆：[动作先验学的是条件速度场](lrp-flow.md)。

[本篇星系](../latent-rl-prior.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/latent-rl-prior.md) · [原文依据](https://arxiv.org/pdf/2611.08458v1)
