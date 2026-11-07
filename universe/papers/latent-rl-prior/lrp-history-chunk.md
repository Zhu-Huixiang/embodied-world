# 历史观测到未来动作块 · Latent RL Prior

H步本体/图像历史条件化K步动作，任务信息压成M个d维context token。

Z_t∈R^{M×d}供动作decoder交叉注意力；R_t走AdaLN条件。H、K、M、d数值及动作维度未在该12页稿给出，不擅套其他模型配置。

[本篇星系](../latent-rl-prior.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/latent-rl-prior.md) · [原文依据](https://arxiv.org/pdf/2611.08458v1)
