# Diffusion Policy 星系

Diffusion Policy: Visuomotor Policy Learning via Action Diffusion

**已精讲** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/diffusion-policy-2303.04137/README.md) · [原文](https://www.roboticsproceedings.org/rss19/p026.html) · [评分卡](../../leaderboard/papers/diffusion-policy/README.md)

对多步动作条件去噪，用视觉观测约束动作分布，滚动执行一段后再次观测与重规划。

## 技术挂点

- [扩散去噪](../concepts/diffusion.md)：训练网络从带噪对象估计噪声或干净目标，生成时从噪声开始迭代恢复样本。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/diffusion-policy-2303.04137/README.md#ii-diffusion-policy-formulation扩散对象变了)

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/diffusion-policy-2303.04137/README.md#a-与-b先把两个时间分清)

- [闭环滚动与历史偏移](../concepts/rollout.md)：重复预测、执行或生成，把新观测或模型历史接回后续计算。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/diffusion-policy-2303.04137/README.md#b-与-c位置控制和执行长度)

- [示范模仿](../concepts/imitation.md)：从专家、人类或教师策略的行为学习动作，研究数据、表示和执行误差。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/diffusion-policy-2303.04137/README.md#i-引言左右都能走怎么偏偏走了中间)

- [机器人数据与评测](../concepts/data.md)：统一观测、动作、任务与评测条件，判断数据多样性如何影响泛化。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/diffusion-policy-2303.04137/README.md#vi-realworld-evaluation到了桌上还能不能顺手)

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/diffusion-policy-2303.04137/README.md#a-网络架构cnn-和-transformer-各干什么)

## 本篇行星与卫星

- [扩散去噪](diffusion-policy/diffusion.md) · 已讲解
- [动作块](diffusion-policy/chunk.md) · 已讲解
- [闭环滚动与历史偏移](diffusion-policy/rollout.md) · 已讲解
- [示范模仿](diffusion-policy/imitation.md) · 已讲解
- [机器人数据与评测](diffusion-policy/data.md) · 已讲解
- [注意力](diffusion-policy/attention.md) · 已讲解
- [本篇方法链路](diffusion-policy/method-chain.md) · 初读挂点
- [动作多模态](diffusion-policy/multimode.md) · 已讲解
- [观察预测执行三窗口](diffusion-policy/horizon.md) · 已讲解
- [动作噪声监督](diffusion-policy/noise.md) · 已讲解
- [固定观察条件](diffusion-policy/condition.md) · 已讲解
- [FiLM与时序Transformer](diffusion-policy/networks.md) · 已讲解
- [视觉空间编码](diffusion-policy/vision.md) · 已讲解
- [动作归一化与旋转](diffusion-policy/normalization.md) · 已讲解
- [滚动执行闭环](diffusion-policy/receding.md) · 已讲解
- [score绕开归一化](diffusion-policy/score.md) · 已讲解
- [checkpoint评估稳定性](diffusion-policy/checkpoint.md) · 已讲解
- [实机终止与底层控制](diffusion-policy/real.md) · 已讲解
- [FiLM通道调制](diffusion-policy/film.md) · 已讲解
- [因果注意力掩码](diffusion-policy/causal-mask.md) · 已讲解
- [空间softmax](diffusion-policy/spatial-softmax.md) · 已讲解
- [分组归一化](diffusion-policy/groupnorm.md) · 已讲解
- [连续6D旋转表示](diffusion-policy/rotation6d.md) · 已讲解
- [DDIM少步采样](diffusion-policy/ddim.md) · 已讲解
- [交并比与终态评估](diffusion-policy/iou.md) · 已讲解

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
