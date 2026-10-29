# DreamerV3 星系

Mastering diverse control tasks through world models

**已精讲** · 世界模型与模型强化学习

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dreamerv3-2301.04104/README.md) · [原文](https://www.nature.com/articles/s41586-025-08744-2) · [评分卡](../../leaderboard/papers/dreamerv3/README.md)

以统一的世界模型、奖励价值尺度处理和优化设计覆盖多类控制任务，减少逐任务调参。

## 技术挂点

- [动作条件动力学](../concepts/dynamics.md)：以当前状态和动作预测下一状态或分布，建立“做这个动作会发生什么”的计算接口。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dreamerv3-2301.04104/README.md#world-model-learning一半记忆一半当前发现)

- [想象轨迹训练](../concepts/imagination.md)：在学到的动力学里滚动状态，用预测奖励和值训练策略，从而增加决策训练数据。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dreamerv3-2301.04104/README.md#critic-learning只想十六步怎么惦记更远的钻石)

- [策略与价值学习](../concepts/actor-critic.md)：actor 产生动作，critic 估计长期收益；价值估计为策略改进提供方向。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dreamerv3-2301.04104/README.md#critic-learning只想十六步怎么惦记更远的钻石)

- [世界模型](../concepts/world.md)：学习状态随动作或时间如何变化，用于预测、计划或训练策略。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dreamerv3-2301.04104/README.md#main别把通用算法读成同一个万能大脑)

- [强化学习](../concepts/rl.md)：通过奖励和值评估改进策略，研究动作如何改变长期回报。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dreamerv3-2301.04104/README.md#actor-learning奖励换了单位探索别跟着抽风)

## 本篇行星与卫星

- [动作条件动力学](dreamerv3/dynamics.md) · 已讲解
- [想象轨迹训练](dreamerv3/imagination.md) · 已讲解
- [策略与价值学习](dreamerv3/actor-critic.md) · 已讲解
- [世界模型](dreamerv3/world.md) · 已讲解
- [强化学习](dreamerv3/rl.md) · 已讲解
- [本篇方法链路](dreamerv3/method-chain.md) · 已讲解
- [循环状态空间模型](dreamerv3/rssm.md) · 已讲解
- [后验与先验](dreamerv3/posterior-prior.md) · 已讲解
- [直通梯度](dreamerv3/straight.md) · 已讲解
- [KL平衡与free bits](dreamerv3/kl.md) · 已讲解
- [潜在空间想象](dreamerv3/imagined-rollout.md) · 已讲解
- [λ-return自举](dreamerv3/lambda.md) · 已讲解
- [回报归一化策略梯度](dreamerv3/actor.md) · 已讲解
- [带符号对数压缩](dreamerv3/symlog.md) · 已讲解
- [symexp two-hot](dreamerv3/twohot.md) · 已讲解
- [Minecraft评测协议](dreamerv3/minecraft.md) · 已讲解
- [表征学习信号消融](dreamerv3/ablation.md) · 已讲解
- [模型规模与交互效率](dreamerv3/scaling.md) · 已讲解
- [分块循环记忆](dreamerv3/blockgru.md) · 已讲解
- [LaProp与梯度裁剪](dreamerv3/laprop.md) · 已讲解
- [经验复用的单位](dreamerv3/replay.md) · 已讲解

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
