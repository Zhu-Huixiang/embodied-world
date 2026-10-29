# Atari表示网络 · MuZero

96×96×128输入压成6×6×256隐藏状态。

32RGB帧加32动作平面；空间48→24→12→6，残差与池化逐段解释。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md#33-atari-的观测到底怎样变成隐藏状态)

继续拆：[动作平面与one-hot](action-plane.md)。

[本篇星系](../muzero.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md) · [原文依据](https://arxiv.org/pdf/1911.08265v2)
