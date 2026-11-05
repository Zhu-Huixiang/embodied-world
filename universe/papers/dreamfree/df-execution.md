# 32步预测与执行窗口 · DreamFree

预测长度、去噪步数和执行长度是三种不同的时钟。

每chunk预测32动作，LIBERO执行10、RoboCasa32、DROID24后再规划。91ms是chunk计算延迟，不能直接当完整观察—执行闭环周期。

[本篇星系](../dreamfree.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamfree.md) · [原文依据](https://arxiv.org/pdf/2611.04527v1)
