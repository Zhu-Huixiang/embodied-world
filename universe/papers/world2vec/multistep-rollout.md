# 沿自身预测轨迹训练多步 · world2vec

从一次编码出发沿记录动作滚动K步，每步对齐真实未来编码。

权重默认1/K；沿自身预测轨迹暴露误差累积，K=1/10/20/40消融要带实际秒数与采样频率。

继续拆：[用正则阻止表示塌缩](regularization.md) · [一致性、LRC与EQA](metrics.md) · [训练视野与动力学参数化消融](ablations.md)。

[本篇星系](../world2vec.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/world2vec.md) · [原文依据](https://arxiv.org/pdf/2610.40637v1)
