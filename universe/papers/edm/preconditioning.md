# 去噪网络预条件化 · EDM

按噪声强度缩放网络输入、输出和跳接，使不同噪声级的训练更稳定。

EDM 用噪声级相关的系数组合跳接输入与网络输出；这与 CLIP 把向量除以 L2 长度是两种操作。

[跨论文技术入口](../../concepts/preconditioning.md)

[本篇星系](../edm.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/edm.md) · [原文依据](https://proceedings.neurips.cc/paper_files/paper/2022/hash/a98846e9d9cc01cfb87eb694d946ce6b-Abstract-Conference.html)
