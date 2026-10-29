# 回放真实轨迹 · MuZero

存真实观测动作奖励及搜索策略/价值。

训练沿回放已经发生的动作展开K5，与树内候选动作来源不同。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md#35-搜索完了谁来教网络)

继续拆：[n步回报与自举](nstep.md) · [联合预测损失](loss.md) · [旧经历重新搜索](reanalyze.md)。

[本篇星系](../muzero.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md) · [原文依据](https://arxiv.org/pdf/1911.08265v2)
