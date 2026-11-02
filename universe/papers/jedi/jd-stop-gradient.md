# 阻止观测支路独自消化辅助损失 · JEDI

将辅助梯度引向压缩器，检查示范slot是否真有用。

当前观测对辅助损失stop-gradient；action loss仍训练policy。Table9放开观测梯度N8成功83.9高于默认80.2，此设计偏向因果隔离而非宣称最高成功率。

[本篇星系](../jedi.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/jedi.md) · [原文依据](https://arxiv.org/pdf/2610.40356v1)
