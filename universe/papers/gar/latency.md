# 动作网络次数与全策略延迟 · GAR

动作网络5/4次减为1次，视觉语言骨干时间仍保留。

RTX4090三session全策略延迟Xiaomi220.25→115.36ms，GR00T68.01→43.30ms；包括预处理、传输、骨干、动作生成与CPU解码，排除通信、排队、模拟器与加载。

[本篇星系](../gar.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/gar.md) · [原文依据](https://arxiv.org/pdf/2610.40271v1)
