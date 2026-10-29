# 行为克隆

直接监督观测到动作的映射，不必在每次更新中根据奖励搜索。

动作块、时序记忆和数据多样性会改变学习难度。

分类上层：[示范模仿](imitation.md)。

## 在完整解读里看计算与例子

- [ACT / ALOHA：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/act-2304.13705/README.md#2-相关工作模仿为什么越做越偏)
- [RT-1：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md#1-引言多练一些任务能帮其他任务吗)

## 哪些论文用到或讨论它

- [ACT / ALOHA](../papers/act.md) · 已精讲 · [原文](https://www.roboticsproceedings.org/rss19/p016.html)
- [RT-1](../papers/rt1.md) · 已精讲 · [原文](https://www.roboticsproceedings.org/rss19/p025.html)
- [robomimic](../papers/robomimic.md) · 机制导读 · [原文](https://proceedings.mlr.press/v164/mandlekar22a.html)
- [BridgeData V2](../papers/bridge-v2.md) · 机制导读 · [原文](https://proceedings.mlr.press/v229/walke23a.html)
- [DROID](../papers/droid.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss20/p120.html)
- [LIBERO](../papers/libero.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2023/hash/8c3c666820ea055a77726d66fc7d447f-Abstract.html)
- [RoboCasa](../papers/robocasa.md) · 机制导读 · [原文](https://roboticsproceedings.org/rss20/p050.html)
- [Mobile ALOHA](../papers/mobile-aloha.md) · 机制导读 · [原文](https://proceedings.mlr.press/v270/fu25b.html)
- [R3M](../papers/r3m.md) · 机制导读 · [原文](https://proceedings.mlr.press/v205/nair23a.html)
- [UMI](../papers/umi.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss20/p045.html)
- [MimicGen](../papers/mimicgen.md) · 机制导读 · [原文](https://proceedings.mlr.press/v229/mandlekar23a.html)
- [Transporter](../papers/transporter.md) · 机制导读 · [原文](https://proceedings.mlr.press/v155/zeng21a.html)
- [IQL](../papers/iql.md) · 机制导读 · [原文](https://iclr.cc/virtual/2022/poster/5941)
- [TD3+BC](../papers/td3-bc.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper/2021/hash/a8166da05c5a094f7dc03724b41886e5-Abstract.html)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
