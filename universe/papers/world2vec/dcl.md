# 起始编码负样本与动态梯度 · world2vec

以起始编码到负样本的距离形成均匀性项。

负样本与起始编码比较而非预测编码；均匀性项只更新编码器，剩余项保持目标有下界并重标预测梯度。

[本篇星系](../world2vec.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/world2vec.md) · [原文依据](https://arxiv.org/pdf/2610.40637v1)
