# 去噪网络预条件化

按噪声强度缩放网络输入、输出和跳接，使不同噪声级的训练更稳定。

EDM 用噪声级相关的系数组合跳接输入与网络输出；这与 CLIP 把向量除以 L2 长度是两种操作。

分类上层：[扩散去噪](diffusion.md)。

## 哪些论文用到或讨论它

- [EDM](../papers/edm.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2022/hash/a98846e9d9cc01cfb87eb694d946ce6b-Abstract-Conference.html)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
