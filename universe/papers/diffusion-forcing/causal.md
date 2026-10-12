# 因果序列建模 · Diffusion Forcing

通过遮罩只让位置读取允许的历史，避免训练时看到运行时不存在的未来。

自回归按顺序产生后续 token；视频和动作的因果粒度需要分别定义。

[跨论文技术入口](../../concepts/causal.md)

[本篇星系](../diffusion-forcing.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/diffusion-forcing.md) · [原文依据](https://proceedings.neurips.cc/paper_files/paper/2024/hash/2aee1c4159e48407d68fe16ae8e6e49e-Abstract-Conference.html)
