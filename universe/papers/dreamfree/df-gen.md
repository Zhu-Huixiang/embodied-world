# 生成流匹配正则 · DreamFree

保留视频模型原有的生成训练目标。

学生当前帧干净、未来帧加噪，预测epsilon-x的速度；生成loss与蒸馏loss相加，不把视频生成留到运行时。

[本篇星系](../dreamfree.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamfree.md) · [原文依据](https://arxiv.org/pdf/2611.04527v1)
