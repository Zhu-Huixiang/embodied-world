# Diffusion Transformer

用 Transformer 实现扩散模型的去噪网络，使 token 之间交换条件与目标信息。

DiT 是网络结构，训练目标及采样器仍要分别说明。

分类上层：[扩散去噪](diffusion.md)。

## 哪些论文用到或讨论它

- [DiT](../papers/dit.md) · 机制导读 · [原文](https://openaccess.thecvf.com/content/ICCV2023/html/Peebles_Scalable_Diffusion_Models_with_Transformers_ICCV_2023_paper.html)
- [ModAR](../papers/modar.md) · 机制导读 · [原文](https://arxiv.org/abs/2609.17524v1)
- [GR00T N1](../papers/gr00t-n1.md) · 机制导读 · [原文](https://arxiv.org/abs/2503.14734)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
