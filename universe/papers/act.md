# ACT / ALOHA 星系

Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware

**已精讲** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/act-2304.13705/README.md) · [原文](https://www.roboticsproceedings.org/rss19/p016.html) · [评分卡](../../leaderboard/papers/act/README.md)

把一段动作联合预测，条件变分自编码器吸收示范差异，时间集成融合重叠预测减轻误差积累。

## 技术挂点

- [变分自编码器 VAE](../concepts/vae.md)：编码器描述潜变量分布，解码器从潜变量重建样本，用重建与分布正则共同训练。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/act-2304.13705/README.md#43-cvae同一幅画面可以有不同的后续走法)

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/act-2304.13705/README.md#41-动作块先预测一小段再决定怎样执行)

- [行为克隆](../concepts/bc.md)：直接监督观测到动作的映射，不必在每次更新中根据奖励搜索。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/act-2304.13705/README.md#2-相关工作模仿为什么越做越偏)

- [示范模仿](../concepts/imitation.md)：从专家、人类或教师策略的行为学习动作，研究数据、表示和执行误差。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/act-2304.13705/README.md#2-相关工作模仿为什么越做越偏)

- [Transformer](../concepts/transformer.md)：用注意力交换 token 信息，再逐位置加工。token 可以来自字词、图像块、状态或动作。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/act-2304.13705/README.md#44-transformer四台相机怎样变成10014)

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/act-2304.13705/README.md#44-transformer四台相机怎样变成10014)

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/act-2304.13705/README.md#4-act-方法动作块时间集成与条件生成)

## 本篇行星与卫星

- [变分自编码器 VAE](act/vae.md) · 已讲解
- [动作块](act/chunk.md) · 已讲解
- [行为克隆](act/bc.md) · 已讲解
- [示范模仿](act/imitation.md) · 已讲解
- [Transformer](act/transformer.md) · 已讲解
- [注意力](act/attention.md) · 已讲解
- [动作表示](act/action.md) · 已讲解
- [本篇方法链路](act/method-chain.md) · 已讲解
- [模仿误差累积](act/compounding-error.md) · 已讲解
- [主从关节遥操作](act/leader-follower.md) · 已讲解
- [四视角观察](act/four-cameras.md) · 已讲解
- [分层控制频率](act/servo-loop.md) · 已讲解
- [目标和实测关节](act/target-vs-measured.md) · 已讲解
- [绝对关节动作](act/absolute-joints.md) · 已讲解
- [块长与有效时域](act/horizon.md) · 已讲解
- [同刻时间集成](act/same-time-ensemble.md) · 已讲解
- [旧预测权重](act/oldest-weight.md) · 已讲解
- [动作潜变量](act/style-latent.md) · 已讲解
- [重参数采样](act/reparameterization.md) · 已讲解
- [高斯KL正则](act/kl-prior.md) · 已讲解
- [L1动作重建](act/l1-reconstruction.md) · 已讲解
- [视觉token形状](act/visual-tokens.md) · 已讲解
- [观察序列融合](act/observation-fusion.md) · 已讲解
- [并行动作查询](act/parallel-action-queries.md) · 已讲解
- [训练汇总token](act/cls-summary.md) · 已讲解
- [逐任务评估协议](act/task-protocol.md) · 已讲解
- [分阶段失败定位](act/stage-failure.md) · 已讲解
- [块长消融](act/chunk-ablation.md) · 已讲解
- [人类示范变化](act/human-variation.md) · 已讲解
- [精细感知瓶颈](act/perception-bottleneck.md) · 已讲解

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
