# 冻结语义编码器，学习运动解码器 · HALO

RGB和语言先变为条件特征，再由DiT生成骨盆相对运动。

Qwen3.5-2B冻结，224×224RGB的64个图像token及文字hidden states从2048维分别投到512维；8层、宽512、8头DiT与投影共训练49.3M参数。

继续拆：[五秒运动写成150乘36](halo-plan.md)。

[本篇星系](../halo.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/halo.md) · [原文依据](https://arxiv.org/pdf/2611.06908v1)
