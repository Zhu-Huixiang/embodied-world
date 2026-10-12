# Trajectory Transformer 星系

Offline Reinforcement Learning as One Big Sequence Modeling Problem

**导读** · 世界模型与模型强化学习

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/trajectory-transformer.md) · [原文](https://proceedings.neurips.cc/paper_files/paper/2021/hash/099fe6b0b444c23836c4a5d07346082b-Abstract.html) · [评分卡](../../leaderboard/papers/trajectory-transformer/README.md)

把状态和动作各维离散化，与奖励串成 token，Transformer 联合学习整段轨迹的概率。规划时用 beam search 保留高回报候选轨迹，执行第一步后重新搜索；稀疏长时序任务还可以接 IQL 的 Q 值做搜索启发。原文同时检查长预测误差、模仿、目标到达与离线 RL。

## 技术挂点

- [因果序列建模](../concepts/causal.md)：通过遮罩只让位置读取允许的历史，避免训练时看到运行时不存在的未来。

- [离散编码与量化](../concepts/quantization.md)：把连续向量或信号映射到有限码。动作、视频潜变量与世界模型状态都可能采用这种表示，码本和训练目标各不相同。

- [树搜索与轨迹搜索](../concepts/search.md)：展开候选动作或轨迹，用预测价值挑选可执行方案。

## 本篇行星与卫星

- [因果序列建模](trajectory-transformer/causal.md) · 初读挂点
- [离散编码与量化](trajectory-transformer/quantization.md) · 初读挂点
- [树搜索与轨迹搜索](trajectory-transformer/search.md) · 初读挂点
- [本篇方法链路](trajectory-transformer/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
