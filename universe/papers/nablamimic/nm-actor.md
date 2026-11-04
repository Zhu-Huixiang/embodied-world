# 参考动作编码与本体历史解码 · ∇Mimic

把未来参考压成低维命令，再结合机器人当前状态产生关节残差。

10×68参考特征经MLP到32维tanh latent；10×93本体历史和6维相对躯干姿态进入解码器；输出29维。

继续拆：[参考姿态加关节残差](nm-residual.md)。

[本篇星系](../nablamimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/nablamimic.md) · [原文依据](https://arxiv.org/pdf/2610.41654v1)
