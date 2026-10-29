# RT-1 星系

RT-1: Robotics Transformer for Real-World Control at Scale

**已精讲** · 视觉语言动作模型 VLA

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md) · [原文](https://www.roboticsproceedings.org/rss19/p025.html) · [评分卡](../../leaderboard/papers/rt1/README.md)

图像先经语言条件的 EfficientNet 提取特征，再由 TokenLearner 压成少量视觉 token；Transformer 融合短时历史并输出离散动作。动作同时覆盖机械臂、底盘和停止模式，策略以闭环方式反复读取图像。原文分别检验新指令、干扰物、新背景以及跨机器人数据混合的效果。

## 技术挂点

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md#51-c-区transformer-输出的是动作档位)

- [离散编码与量化](../concepts/quantization.md)：把连续向量或信号映射到有限码。动作、视频潜变量与世界模型状态都可能采用这种表示，码本和训练目标各不相同。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md#51-c-区transformer-输出的是动作档位)

- [跨本体数据](../concepts/cross-body.md)：从多个机器人或人类收集经验，通过动作/观测适配接到共享学习系统。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md#63-仿真数据能不能搬到现实)

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md#51-a-区语言先改看法再决定做法)

- [Transformer](../concepts/transformer.md)：用注意力交换 token 信息，再逐位置加工。token 可以来自字词、图像块、状态或动作。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md#51-c-区transformer-输出的是动作档位)

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md#3-问题定义一句指令不等于一整套计划)

- [交叉熵](../concepts/cross-entropy.md)：正确候选的负对数概率。正确项概率越小，损失越大，梯度会推动正确分数上升。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md#52-d-区监督的答案就是人类当时选的动作)

- [示范模仿](../concepts/imitation.md)：从专家、人类或教师策略的行为学习动作，研究数据、表示和执行误差。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md#52-d-区监督的答案就是人类当时选的动作)

- [行为克隆](../concepts/bc.md)：直接监督观测到动作的映射，不必在每次更新中根据奖励搜索。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md#1-引言多练一些任务能帮其他任务吗)

- [机器人数据与评测](../concepts/data.md)：统一观测、动作、任务与评测条件，判断数据多样性如何影响泛化。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md#4-系统概览数据究竟从哪里来)

- [仿真到实机](../concepts/sim2real.md)：处理仿真动力学、感知和真实系统间的差异，通过随机化、辨识、残差或适配来迁移。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md#63-仿真数据能不能搬到现实)

- [分层技能与计划](../concepts/skills.md)：高层选择目标或技能，低层负责具体执行，层次之间有明确接口。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md#64-长程任务把想做什么和做没做成拆开)

- [闭环滚动与历史偏移](../concepts/rollout.md)：重复预测、执行或生成，把新观测或模型历史接回后续计算。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md#53-e-区动作算出来要赶得上现场)

## 本篇行星与卫星

- [注意力](rt1/attention.md) · 已讲解
- [离散编码与量化](rt1/quantization.md) · 已讲解
- [跨本体数据](rt1/cross-body.md) · 已讲解
- [表征空间](rt1/representation.md) · 已讲解
- [Transformer](rt1/transformer.md) · 已讲解
- [动作表示](rt1/action.md) · 已讲解
- [交叉熵](rt1/cross-entropy.md) · 已讲解
- [示范模仿](rt1/imitation.md) · 已讲解
- [行为克隆](rt1/bc.md) · 已讲解
- [机器人数据与评测](rt1/data.md) · 已讲解
- [仿真到实机](rt1/sim2real.md) · 已讲解
- [分层技能与计划](rt1/skills.md) · 已讲解
- [闭环滚动与历史偏移](rt1/rollout.md) · 已讲解
- [本篇方法链路](rt1/method-chain.md) · 已讲解
- [语言调制视觉](rt1/rt1-film.md) · 已讲解
- [学习视觉摘要](rt1/rt1-tokenlearner.md) · 已讲解
- [六帧观察历史](rt1/rt1-history.md) · 已讲解
- [连续动作分类化](rt1/rt1-action-bins.md) · 已讲解
- [动作非自回归输出](rt1/rt1-nonar.md) · 已讲解
- [逐动作模仿监督](rt1/rt1-loss.md) · 已讲解
- [闭环时延预算](rt1/rt1-latency.md) · 已讲解
- [拆分泛化因素](rt1/rt1-gen-tests.md) · 已讲解
- [混合仿真迁移](rt1/rt1-mixedsim.md) · 已讲解
- [跨机器人数据桥](rt1/rt1-mixedbody.md) · 已讲解
- [高低层分工](rt1/rt1-saycan.md) · 已讲解
- [采集覆盖与数量](rt1/rt1-coverage.md) · 已讲解

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
