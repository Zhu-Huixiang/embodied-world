# 当前两帧与未来十六帧分开编码 · La-JEPA

当前观测不能从未来视频编码中偷看答案。

当前(t−1,t)两帧给一个空间网格；未来t+2至t+32间隔2采16帧，由两帧tubelet得到8个时间网格。未来帧可联合注意，但当前片段独立编码；tube-motion是最终方案。

继续拆：[平均与拼接都减少token，但保留信息不同](la-jepa-spatial.md)。

[本篇星系](../la-jepa.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/la-jepa.md) · [原文依据](https://arxiv.org/pdf/2611.08156v1)
