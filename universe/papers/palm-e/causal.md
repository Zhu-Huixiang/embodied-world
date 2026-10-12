# 因果序列建模 · PaLM-E

通过遮罩只让位置读取允许的历史，避免训练时看到运行时不存在的未来。

自回归按顺序产生后续 token；视频和动作的因果粒度需要分别定义。

[跨论文技术入口](../../concepts/causal.md)

[本篇星系](../palm-e.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/palm-e.md) · [原文依据](https://proceedings.mlr.press/v202/driess23a.html)
