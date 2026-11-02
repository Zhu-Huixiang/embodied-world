# 每条示范独立压成八个slot · JEDI

示范独立压缩允许重复查询时复用缓存。

8采样帧×双视角SigLIP视觉token和128状态/动作步输入4层联合Perceiver，输出k8固定slot。token带视角、模态及归一时间，slot无示范身份编码。

继续拆：[预测查询回合的下一关键帧](jd-query-future.md) · [Flow Matching动作专家](jd-action-expert.md) · [更多上下文与分布偏移](jd-many-shot.md) · [缓存控制率与bank建立代价](jd-cost.md) · [视觉patch输入与预测目标的维度](jd-vision-tokens.md)。

[本篇星系](../jedi.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/jedi.md) · [原文依据](https://arxiv.org/pdf/2610.40356v1)
