# MuZero 星系

Mastering Atari, Go, chess and shogi by planning with a learned model

**已精讲** · 世界模型与模型强化学习

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md) · [原文](https://www.nature.com/articles/s41586-020-03051-4) · [评分卡](../../leaderboard/papers/muzero/README.md)

表示网络从观测历史得到潜状态，动力学网络在动作条件下预测下一潜状态和奖励，预测网络给出策略先验和值。MCTS 在这些潜状态里展开候选动作，搜索产生的策略和值再监督网络。Nature 论文比较棋类与 Atari；这里关注的是规划表征，而不是实机机器人结论。

## 技术挂点

- [动作条件动力学](../concepts/dynamics.md)：以当前状态和动作预测下一状态或分布，建立“做这个动作会发生什么”的计算接口。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md#32-hgf各自接什么吐什么)

- [树搜索与轨迹搜索](../concepts/search.md)：展开候选动作或轨迹，用预测价值挑选可执行方案。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md#34-一次搜索挑路扩一格往回记账)

- [价值估计与校准](../concepts/value.md)：估计未来累积收益，再用保守、分位或参考价值等约束减少误导。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md#35-搜索完了谁来教网络)

- [世界模型](../concepts/world.md)：学习状态随动作或时间如何变化，用于预测、计划或训练策略。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md#1-引言会做决定得先会复刻世界吗)

- [强化学习](../concepts/rl.md)：通过奖励和值评估改进策略，研究动作如何改变长期回报。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md#35-搜索完了谁来教网络)

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md#33-atari-的观测到底怎样变成隐藏状态)

- [交叉熵](../concepts/cross-entropy.md)：正确候选的负对数概率。正确项概率越小，损失越大，梯度会推动正确分数上升。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md#36-损失函数三份作业一起改hgf)

- [闭环滚动与历史偏移](../concepts/rollout.md)：重复预测、执行或生成，把新观测或模型历史接回后续计算。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md#34-一次搜索挑路扩一格往回记账)

## 本篇行星与卫星

- [动作条件动力学](muzero/dynamics.md) · 已讲解
- [树搜索与轨迹搜索](muzero/search.md) · 已讲解
- [价值估计与校准](muzero/value.md) · 已讲解
- [世界模型](muzero/world.md) · 已讲解
- [强化学习](muzero/rl.md) · 已讲解
- [表征空间](muzero/representation.md) · 已讲解
- [交叉熵](muzero/cross-entropy.md) · 已讲解
- [闭环滚动与历史偏移](muzero/rollout.md) · 已讲解
- [本篇方法链路](muzero/method-chain.md) · 初读挂点
- [任务相关模型](muzero/task-model.md) · 已讲解
- [精确模型与价值等价前史](muzero/predecessors.md) · 已讲解
- [h/g/f三个接口](muzero/hgf.md) · 已讲解
- [Atari表示网络](muzero/representation-shape.md) · 已讲解
- [动作平面与one-hot](muzero/action-plane.md) · 已讲解
- [601点奖励价值分布](muzero/support.md) · 已讲解
- [模型内树搜索](muzero/mcts.md) · 已讲解
- [pUCT选择](muzero/puct.md) · 已讲解
- [叶节点扩张](muzero/expand.md) · 已讲解
- [折扣回传与均值](muzero/backup.md) · 已讲解
- [访问次数转策略](muzero/visits.md) · 已讲解
- [根合法动作与内部模型](muzero/legal.md) · 已讲解
- [回放真实轨迹](muzero/replay.md) · 已讲解
- [n步回报与自举](muzero/nstep.md) · 已讲解
- [联合预测损失](muzero/loss.md) · 已讲解
- [软分布交叉熵](muzero/ce.md) · 已讲解
- [展开梯度缩放](muzero/grad.md) · 已讲解
- [旧经历重新搜索](muzero/reanalyze.md) · 已讲解
- [更新次数与棋力曲线](muzero/curves.md) · 已讲解
- [人类归一化分数](muzero/hns.md) · 已讲解
- [分预算比较Atari](muzero/budget.md) · 已讲解
- [评估搜索预算消融](muzero/eval-search.md) · 已讲解
- [同框架Q学习对照](muzero/q-baseline.md) · 已讲解
- [训练搜索老师的预算](muzero/train-search.md) · 已讲解
- [训练展开不封顶树深](muzero/depth.md) · 已讲解
- [搜索经验进入策略网络](muzero/prior-search.md) · 已讲解
- [单游戏失败与稀疏奖励](muzero/failures.md) · 已讲解
- [连续动作与真实代价](muzero/robotics.md) · 已讲解

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
