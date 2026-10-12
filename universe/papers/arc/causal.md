# 因果序列建模 · ARC

通过遮罩只让位置读取允许的历史，避免训练时看到运行时不存在的未来。

自回归按顺序产生后续 token；视频和动作的因果粒度需要分别定义。

[跨论文技术入口](../../concepts/causal.md)

[本篇星系](../arc.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/arc.md) · [原文依据](https://arxiv.org/abs/2610.12386v1)
