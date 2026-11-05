# 1B动作DiT流匹配 · DreamFree

在动作空间迭代求解速度场。

约1B解码器由30个DiT块构成，条件为视觉readout、指令和本体状态；使用32步动作chunk，LIBERO/RoboCasa10个Euler步，DROID16步，无CFG。

继续拆：[DROID八步动作历史](df-history.md) · [32步预测与执行窗口](df-execution.md)。

[本篇星系](../dreamfree.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamfree.md) · [原文依据](https://arxiv.org/pdf/2611.04527v1)
