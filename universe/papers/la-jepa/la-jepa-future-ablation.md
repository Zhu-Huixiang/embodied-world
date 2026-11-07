# 未来监督的收益要在同一管线内看 · La-JEPA

去掉future损失与计算，保留action路径作为对照。

LIBERO-Plus原始管线三seed均值76.47%对action-only74.35%，每seed配对McNemar p<0.01；这组不能与修订管线主表88.0%直接比。RoboTwin单次训练为80.16/39.02对73.14/35.34（clean/randomized），每条件5000回合，checkpoint不同。

继续拆：[JEPA与VAE比的是表征系统](la-jepa-feature-space.md)。

[本篇星系](../la-jepa.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/la-jepa.md) · [原文依据](https://arxiv.org/pdf/2611.08156v1)
