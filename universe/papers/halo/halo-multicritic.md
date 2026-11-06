# 共享演员，分开评价不同技能 · HALO

蒸馏后以多critic PPO继续优化共享学生。

每个技能族保留独立critic并分别标准化优势，训练使用16384环境、4张H100；共享actor再加入扰动和15–40ms延迟随机化。

[本篇星系](../halo.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/halo.md) · [原文依据](https://arxiv.org/pdf/2611.06908v1)
