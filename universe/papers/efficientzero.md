# EfficientZero 星系

Mastering Atari Games with Limited Data

**导读** · 世界模型与模型强化学习

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/efficientzero.md) · [原文](https://proceedings.neurips.cc/paper/2021/hash/d5eca8dc3820cad9fe56a3bafda65ca1-Abstract.html) · [评分卡](../../leaderboard/papers/efficientzero/README.md)

编码器把图像变成潜状态，动力学网络预测下一潜状态，MCTS 在这个模型里比较动作。EfficientZero 用预测潜状态与真实下一帧编码的一致性补强动力学监督，预测累计价值前缀，并重分析旧数据来缓解离策略目标偏差。它测试的是有限交互预算下的游戏与模拟控制效率。

## 技术挂点

- [动作条件动力学](../concepts/dynamics.md)：以当前状态和动作预测下一状态或分布，建立“做这个动作会发生什么”的计算接口。

- [树搜索与轨迹搜索](../concepts/search.md)：展开候选动作或轨迹，用预测价值挑选可执行方案。

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。

## 本篇行星与卫星

- [动作条件动力学](efficientzero/dynamics.md) · 初读挂点
- [树搜索与轨迹搜索](efficientzero/search.md) · 初读挂点
- [表征空间](efficientzero/representation.md) · 初读挂点
- [本篇方法链路](efficientzero/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
