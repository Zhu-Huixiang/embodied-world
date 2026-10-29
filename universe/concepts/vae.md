# 变分自编码器 VAE

编码器描述潜变量分布，解码器从潜变量重建样本，用重建与分布正则共同训练。

ACT 中潜变量表达示范差异；不要把任何 latent 都叫 VAE。

分类上层：[条件生成](generation.md)。

## 哪些论文用到或讨论它

- [ACT / ALOHA](../papers/act.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss19/p016.html)
- [DreamWaQ](../papers/dreamwaq.md) · 机制导读 · [原文](https://ieeexplore.ieee.org/abstract/document/10161144/)
- [LingBot-VA](../papers/lingbot-va.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss22/p016.html)
- [JAM](../papers/jam.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.37219v1)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
