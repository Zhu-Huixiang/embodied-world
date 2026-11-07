# 两个独立流时间，两个速度目标 · La-JEPA

未来特征与动作都从高斯噪声插值到干净目标。

分别采τf和τa∈U(0,1)，zτf=(1−τf)εf+τfzfut，Aτa=(1−τa)εa+τaA；速度目标为zfut−εf和A−εa，两项MSE各权重1并按各自元素平均。

继续拆：[部署删未来，再缓存观测键值](la-jepa-inference.md) · [未来监督的收益要在同一管线内看](la-jepa-future-ablation.md)。

[本篇星系](../la-jepa.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/la-jepa.md) · [原文依据](https://arxiv.org/pdf/2611.08156v1)
