# 闭环滚动与历史偏移

重复预测、执行或生成，把新观测或模型历史接回后续计算。

Teacher forcing 与运行时自有历史之间的差异需单独检查。

分类上层：[视频时序生成](video.md)。

## 在完整解读里看计算与例子

- [Diffusion Policy：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/diffusion-policy-2303.04137/README.md#b-与-c位置控制和执行长度)
- [MuZero：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md#34-一次搜索挑路扩一格往回记账)

## 哪些论文用到或讨论它

- [Diffusion Policy](../papers/diffusion-policy.md) · 已精讲 · [原文](https://www.roboticsproceedings.org/rss19/p026.html)
- [LingBot-VA](../papers/lingbot-va.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss22/p016.html)
- [Self Forcing](../papers/self-forcing.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2025/hash/f4823f831af67a3ef15e41a85434422a-Abstract-Conference.html)
- [DayDreamer](../papers/daydreamer.md) · 机制导读 · [原文](https://proceedings.mlr.press/v205/wu23c.html)
- [MuZero](../papers/muzero.md) · 已精讲 · [原文](https://www.nature.com/articles/s41586-020-03051-4)
- [Walk in the Park](../papers/walk-in-the-park.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss19/p056.html)
- [SAM 2](../papers/sam2.md) · 机制导读 · [原文](https://openreview.net/forum?id=Ha6RTeWMd0)
- [Ctrl-World](../papers/ctrl-world.md) · 机制导读 · [原文](https://proceedings.iclr.cc/paper_files/paper/2026/hash/0ae94013da7cd459402fd77874e09ee3-Abstract-Conference.html)
- [DiffContact](../papers/diffcontact.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.35852v1)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
