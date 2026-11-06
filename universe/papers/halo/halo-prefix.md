# 把已承诺的半秒作为干净前缀 · HALO

首15帧始终干净，网络只学习后135帧如何接续。

前缀逐帧流时间设1，损失只在未来135帧并按36×135归一；推理每一步覆盖回原前缀，3Hz异步更新计划。参考接缝连续，不等于执行必然稳定或安全。

继续拆：[异步前缀接续影响是否能坐下](halo-rtc-ablation.md)。

[本篇星系](../halo.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/halo.md) · [原文依据](https://arxiv.org/pdf/2611.06908v1)
