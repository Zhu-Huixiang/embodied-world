# 动作块

一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。

块长、执行长度和重新观测频率可以不同。

分类上层：[动作表示](action.md)。

## 在完整解读里看计算与例子

- [ACT / ALOHA：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/act-2304.13705/README.md#41-动作块先预测一小段再决定怎样执行)
- [DDPM：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md#6-三个问题再落到机器人动作上)
- [Diffusion Policy：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/diffusion-policy-2303.04137/README.md#a-与-b先把两个时间分清)
- [Holo-M：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md#31-统一动作编码208究竟怎么算出来的)

## 哪些论文用到或讨论它

- [Holo-M](../papers/holo-m.md) · 已精讲 · [原文](https://arxiv.org/abs/2609.35709v1)
- [π₀](../papers/pi0.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss21/p010.html)
- [Diffusion Policy](../papers/diffusion-policy.md) · 已精讲 · [原文](https://www.roboticsproceedings.org/rss19/p026.html)
- [ACT / ALOHA](../papers/act.md) · 已精讲 · [原文](https://www.roboticsproceedings.org/rss19/p016.html)
- [DP3](../papers/dp3.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss20/p067.html)
- [Consistency Policy](../papers/consistency-policy.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss20/p071.html)
- [Octo](../papers/octo.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss20/p090.html)
- [Mobile ALOHA](../papers/mobile-aloha.md) · 机制导读 · [原文](https://proceedings.mlr.press/v270/fu25b.html)
- [DDPM](../papers/ddpm.md) · 已精讲 · [原文](https://proceedings.neurips.cc/paper/2020/hash/4c5bcfec8584af0d967f1ab10179ca4b-Abstract.html)
- [FLoRe](../papers/flore.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.35862v1)
- [JAM](../papers/jam.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.37219v1)
- [TOPS](../papers/tops.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.36694v1)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
