# 两份数据不要求轨迹配对 · Latent RL Prior

预训练数据含特权状态、本体和动作；视觉适配数据含图像、本体和动作。

D_RL={(P_t,R_t,A_t)}，D_vis={(I_t,R_t,A_t)}；后者无特权标签、无预训练latent目标，不需与前者逐条配对。

继续拆：[历史观测到未来动作块](lrp-history-chunk.md) · [先收集十万条成功RL轨迹](lrp-teacher.md)。

[本篇星系](../latent-rl-prior.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/latent-rl-prior.md) · [原文依据](https://arxiv.org/pdf/2611.08458v1)
