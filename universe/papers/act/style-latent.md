# 动作潜变量 · ACT / ALOHA

训练编码器把示范差异压入32维高斯潜变量。

只读关节和动作块，部署去掉编码器并固定z0。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/act-2304.13705/README.md#43-cvae同一幅画面可以有不同的后续走法)

继续拆：[重参数采样](reparameterization.md) · [高斯KL正则](kl-prior.md) · [L1动作重建](l1-reconstruction.md) · [训练汇总token](cls-summary.md) · [人类示范变化](human-variation.md)。

[本篇星系](../act.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/act-2304.13705/README.md) · [原文依据](https://www.roboticsproceedings.org/rss19/p016.html)
