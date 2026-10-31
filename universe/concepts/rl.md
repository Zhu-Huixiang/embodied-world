# 强化学习

通过奖励和值评估改进策略，研究动作如何改变长期回报。

状态、动作、奖励、回报与价值不要混成一个数。

继续拆：[策略与价值学习](actor-critic.md) · [离线强化学习](offline.md) · [PPO 与并行模拟](ppo.md) · [环境适应](adaptation.md)。

## 在完整解读里看计算与例子

- [DreamerV3：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dreamerv3-2301.04104/README.md#actor-learning奖励换了单位探索别跟着抽风)
- [MuZero：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md#35-搜索完了谁来教网络)
- [RMA：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md#31-基础策略特权信息怎样教出一套步态)

## 哪些论文用到或讨论它

- [RMA](../papers/rma.md) · 已精讲 · [原文](https://www.roboticsproceedings.org/rss17/p011.html)
- [DeepMimic](../papers/deepmimic.md) · 机制导读 · [原文](https://xbpeng.github.io/projects/DeepMimic/)
- [AMP](../papers/amp.md) · 机制导读 · [原文](https://xbpeng.github.io/projects/AMP/)
- [DreamerV3](../papers/dreamerv3.md) · 已精讲 · [原文](https://www.nature.com/articles/s41586-025-08744-2)
- [VIP](../papers/vip.md) · 机制导读 · [原文](https://openreview.net/forum?id=YJ7o2wetJ2)
- [MuZero](../papers/muzero.md) · 已精讲 · [原文](https://www.nature.com/articles/s41586-020-03051-4)
- [Deep WBC](../papers/deep-whole-body-control.md) · 机制导读 · [原文](https://proceedings.mlr.press/v205/fu23a.html)
- [Isaac Gym](../papers/isaac-gym.md) · 机制导读 · [原文](https://datasets-benchmarks-proceedings.neurips.cc/paper/2021/hash/28dd2c7955ce926456240b2ff0100bde-Abstract-round2.html)
- [DiffContact](../papers/diffcontact.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.35852v1)
- [Dex-One2Many](../papers/dex-one2many.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.12470v1)
- [Balanced Data Diet](../papers/balanced-data-diet.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.12465v1)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
