# Decision Transformer 星系

Decision Transformer: Reinforcement Learning via Sequence Modeling

**导读** · 强化学习与离线决策

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/decision-transformer.md) · [原文](https://proceedings.neurips.cc/paper_files/paper/2021/hash/7f489f642a0ddb10272b5c31057f0663-Abstract.html) · [评分卡](../../leaderboard/papers/decision-transformer/README.md)

把未来目标回报、状态和动作按时间交错成序列，因果 Transformer 用过去上下文预测当前动作。训练直接拟合数据动作；执行后减去已经获得的奖励，再把更新后的目标回报与新状态送回模型。实验用 Atari、Gym 与长时序任务检验这个条件生成式策略。

## 技术挂点

- [因果序列建模](../concepts/causal.md)：通过遮罩只让位置读取允许的历史，避免训练时看到运行时不存在的未来。

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

- [离线强化学习](../concepts/offline.md)：从已有轨迹学习决策，训练时不能自由去环境补齐数据外动作的后果。

## 本篇行星与卫星

- [因果序列建模](decision-transformer/causal.md) · 初读挂点
- [动作表示](decision-transformer/action.md) · 初读挂点
- [离线强化学习](decision-transformer/offline.md) · 初读挂点
- [本篇方法链路](decision-transformer/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
