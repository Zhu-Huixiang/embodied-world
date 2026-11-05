# 未来token余弦蒸馏 · DreamFree

只在未来位置比较教师与学生对齐输出。

双方去掉当前位置，非仿射LayerNorm后取平均余弦距离；实现1-sim与正文-sim只差常数。教师和projector部署时都丢弃。

[本篇星系](../dreamfree.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamfree.md) · [原文依据](https://arxiv.org/pdf/2611.04527v1)
