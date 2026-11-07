# 用人接管前的状态定阈值 · OopsieRecover

触发尺度从真实干预记录校准，而非由VLM随意报阈值。

所读v1 Eq4在每次干预前且gate=1的状态中取最低gate score，再跨同类记录取最小值；部署分数大于阈值才触发。

继续拆：[回放检查只检查已有纠正方向](oopsierecover-verification.md)。

[本篇星系](../oopsierecover.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/oopsierecover.md) · [原文依据](https://arxiv.org/pdf/2611.08462v1)
