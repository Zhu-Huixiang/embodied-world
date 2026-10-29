# 因果序列建模

通过遮罩只让位置读取允许的历史，避免训练时看到运行时不存在的未来。

自回归按顺序产生后续 token；视频和动作的因果粒度需要分别定义。

分类上层：[注意力](attention.md)。

## 在完整解读里看计算与例子

- [Transformer：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md#5-训练答案右移未来遮住)

## 哪些论文用到或讨论它

- [FAST](../papers/fast.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss21/p012.html)
- [RT-2](../papers/rt2.md) · 机制导读 · [原文](https://proceedings.mlr.press/v229/zitkovich23a.html)
- [CoT-VLA](../papers/cot-vla.md) · 机制导读 · [原文](https://openaccess.thecvf.com/content/CVPR2025/html/Zhao_CoT-VLA_Visual_Chain-of-Thought_Reasoning_for_Vision-Language-Action_Models_CVPR_2025_paper.html)
- [LingBot-VA](../papers/lingbot-va.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss22/p016.html)
- [Diffusion Forcing](../papers/diffusion-forcing.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2024/hash/2aee1c4159e48407d68fe16ae8e6e49e-Abstract-Conference.html)
- [Self Forcing](../papers/self-forcing.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2025/hash/f4823f831af67a3ef15e41a85434422a-Abstract-Conference.html)
- [PaLM-E](../papers/palm-e.md) · 机制导读 · [原文](https://proceedings.mlr.press/v202/driess23a.html)
- [VIMA](../papers/vima.md) · 机制导读 · [原文](https://proceedings.mlr.press/v202/jiang23b.html)
- [VQ-BeT](../papers/vq-bet.md) · 机制导读 · [原文](https://proceedings.mlr.press/v235/lee24y.html)
- [Decision Transformer](../papers/decision-transformer.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2021/hash/7f489f642a0ddb10272b5c31057f0663-Abstract.html)
- [Trajectory Transformer](../papers/trajectory-transformer.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2021/hash/099fe6b0b444c23836c4a5d07346082b-Abstract.html)
- [Transformer](../papers/attention.md) · 已精讲 · [原文](https://papers.nips.cc/paper/2017/hash/3f5ee243547dee91fbd053c1c4a845aa-Abstract.html)
- [ModAR](../papers/modar.md) · 机制导读 · [原文](https://arxiv.org/abs/2609.17524v1)
- [ARC](../papers/arc.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.12386v1)
- [PLaW-VLA](../papers/plaw-vla.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.12285v1)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
