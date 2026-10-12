# 因果序列建模 · Self Forcing

通过遮罩只让位置读取允许的历史，避免训练时看到运行时不存在的未来。

自回归按顺序产生后续 token；视频和动作的因果粒度需要分别定义。

[跨论文技术入口](../../concepts/causal.md)

[本篇星系](../self-forcing.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/self-forcing.md) · [原文依据](https://proceedings.neurips.cc/paper_files/paper/2025/hash/f4823f831af67a3ef15e41a85434422a-Abstract-Conference.html)
