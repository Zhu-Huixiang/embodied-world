# world2vec 星系

world2vec: Mechanistic world models through latent dynamics learning

**导读** · 世界模型与模型强化学习

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/world2vec.md) · [原文](https://arxiv.org/abs/2610.40637v1) · [评分卡](../../leaderboard/papers/world2vec/README.md)

world2vec用三帧观测编码潜状态，MLP预测动作条件变化率，以Euler残差积分出多步潜轨迹；把每一步预测对齐真实未来编码，以SIGReg或DCL防止表示塌缩。超参选择用未来检索EQA，另报告跨seed仿射一致性和LRC。执行时编码目标观测，CEM按潜距离选动作并滚动重规划，不训练奖励模型。科学辨识实验另将向量场换成稀疏多项式库，在已知最高阶和仿射坐标不确定性下读出动力学关系。

## 技术挂点

- [世界模型](../concepts/world.md)：学习状态随动作或时间如何变化，用于预测、计划或训练策略。

- [动作条件动力学](../concepts/dynamics.md)：以当前状态和动作预测下一状态或分布，建立“做这个动作会发生什么”的计算接口。

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。

- [表征预测 JEPA](../concepts/jepa.md)：在表征空间预测目标而不是逐像素重建；防止表征坍缩仍需要相应设计。

- [对比学习](../concepts/contrastive.md)：给相关样本较高相似度，让它们在候选竞争中被找回来。图文配对是 CLIP 的监督来源。

- [Transformer](../concepts/transformer.md)：用注意力交换 token 信息，再逐位置加工。token 可以来自字词、图像块、状态或动作。

- [视觉 patch token](../concepts/patches.md)：把图像切成块，展平并投影成向量，再加入位置信息。

- [闭环滚动与历史偏移](../concepts/rollout.md)：重复预测、执行或生成，把新观测或模型历史接回后续计算。

- [模型预测控制 MPC](../concepts/mpc.md)：在模型里比较未来动作序列，执行开头一段，用新观测重算下一轮。

- [树搜索与轨迹搜索](../concepts/search.md)：展开候选动作或轨迹，用预测价值挑选可执行方案。

- [离线强化学习](../concepts/offline.md)：从已有轨迹学习决策，训练时不能自由去环境补齐数据外动作的后果。

- [逆动力学](../concepts/inverse.md)：从状态变化或相邻画面推回可能的动作，给视频计划连接环境专用执行接口。

- [泛化评测与遗忘](../concepts/benchmark.md)：拆开任务、物体、场景或学习顺序，检查迁移能力和旧技能保留。

## 本篇行星与卫星

- [世界模型](world2vec/world.md) · 初读挂点
- [动作条件动力学](world2vec/dynamics.md) · 初读挂点
- [表征空间](world2vec/representation.md) · 初读挂点
- [表征预测 JEPA](world2vec/jepa.md) · 初读挂点
- [对比学习](world2vec/contrastive.md) · 初读挂点
- [Transformer](world2vec/transformer.md) · 初读挂点
- [视觉 patch token](world2vec/patches.md) · 初读挂点
- [闭环滚动与历史偏移](world2vec/rollout.md) · 初读挂点
- [模型预测控制 MPC](world2vec/mpc.md) · 初读挂点
- [树搜索与轨迹搜索](world2vec/search.md) · 初读挂点
- [离线强化学习](world2vec/offline.md) · 初读挂点
- [逆动力学](world2vec/inverse.md) · 初读挂点
- [泛化评测与遗忘](world2vec/benchmark.md) · 初读挂点
- [本篇方法链路](world2vec/method-chain.md) · 初读挂点
- [高任务回报与忠实动力学](world2vec/objective.md) · 初读挂点
- [编码与时间演化可交换](world2vec/faithfulness.md) · 初读挂点
- [三帧历史补充速度信息](world2vec/history.md) · 初读挂点
- [潜向量场与Euler残差](world2vec/euler.md) · 初读挂点
- [沿自身预测轨迹训练多步](world2vec/multistep-rollout.md) · 初读挂点
- [用正则阻止表示塌缩](world2vec/regularization.md) · 初读挂点
- [SIGReg的一维投影分布约束](world2vec/sigreg.md) · 初读挂点
- [起始编码负样本与动态梯度](world2vec/dcl.md) · 初读挂点
- [一致性、LRC与EQA](world2vec/metrics.md) · 初读挂点
- [目标编码与CEM规划](world2vec/latent-mpc.md) · 初读挂点
- [目标帧与Reacher逆运动学](world2vec/goals.md) · 初读挂点
- [随机动作视觉数据与切分](world2vec/dataset.md) · 初读挂点
- [三项仿真控制的收益和失败](world2vec/control-evidence.md) · 初读挂点
- [LeWM原目标到达协议](world2vec/goal-protocol.md) · 初读挂点
- [训练视野与动力学参数化消融](world2vec/ablations.md) · 初读挂点
- [改变积分步长与控制频率](world2vec/retiming.md) · 初读挂点
- [潜空间几何与非线性混合](world2vec/geometry.md) · 初读挂点
- [稀疏多项式潜动力学](world2vec/sindy.md) · 初读挂点
- [71个受控混合动力系统](world2vec/attractors.md) · 初读挂点
- [过程噪声与可辨识性](world2vec/noise-identifiability.md) · 初读挂点
- [在验证集选参并报告验证集](world2vec/validation-boundary.md) · 初读挂点
- [最佳示例的对齐与系数阈值](world2vec/symbolic-showcase.md) · 初读挂点
- [复用与外推边界](world2vec/limits.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
