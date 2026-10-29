# 离散编码与量化

把连续向量或信号映射到有限码。动作、视频潜变量与世界模型状态都可能采用这种表示，码本和训练目标各不相同。

量化误差与码序列长度要同时观察。

分类上层：[动作表示](action.md)。

继续拆：[残差向量量化 RVQ](rvq.md)。

## 在完整解读里看计算与例子

- [RT-1：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md#51-c-区transformer-输出的是动作档位)

## 哪些论文用到或讨论它

- [FAST](../papers/fast.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss21/p012.html)
- [OpenVLA](../papers/openvla.md) · 机制导读 · [原文](https://proceedings.mlr.press/v270/kim25c.html)
- [RT-2](../papers/rt2.md) · 机制导读 · [原文](https://proceedings.mlr.press/v229/zitkovich23a.html)
- [DreamerV2](../papers/dreamerv2.md) · 机制导读 · [原文](https://research.google/pubs/mastering-atari-with-discrete-world-models/)
- [RT-1](../papers/rt1.md) · 已精讲 · [原文](https://www.roboticsproceedings.org/rss19/p025.html)
- [VQ-BeT](../papers/vq-bet.md) · 机制导读 · [原文](https://proceedings.mlr.press/v235/lee24y.html)
- [Trajectory Transformer](../papers/trajectory-transformer.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2021/hash/099fe6b0b444c23836c4a5d07346082b-Abstract.html)
- [Phenaki](../papers/phenaki.md) · 机制导读 · [原文](https://openreview.net/forum?id=vOEXS39nOF)
- [SONIC](../papers/sonic.md) · 机制导读 · [原文](https://www.science.org/doi/10.1126/scirobotics.aed4592)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
