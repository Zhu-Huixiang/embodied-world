# 71个受控混合动力系统 · world2vec

对dysts混沌系统加入过程噪声并做非线性观测混合。

每系统1000条×1000步，RK4与系统相关步长，固定四层注入MLP投到50维；按轨迹70/15/15切分，K1、三seed、10k迭代。不是71个机器人任务。

继续拆：[过程噪声与可辨识性](noise-identifiability.md) · [在验证集选参并报告验证集](validation-boundary.md)。

[本篇星系](../world2vec.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/world2vec.md) · [原文依据](https://arxiv.org/pdf/2610.40637v1)
