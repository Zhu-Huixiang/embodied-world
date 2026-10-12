# R3M 星系

R3M: A Universal Visual Representation for Robot Manipulation

**导读** · 具身感知与场景表示

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/r3m.md) · [原文](https://proceedings.mlr.press/v205/nair23a.html) · [评分卡](../../leaderboard/papers/r3m/README.md)

在人类视频上联合时间对比、视频语言对齐和稀疏约束，让编码器同时记住场景变化与任务语义。下游冻结编码器，把图像向量交给机器人策略，只用少量机器人示范学习动作。原文比较从零训练、CLIP、MoCo 等视觉初始化，并在真实公寓中测试操作。

## 技术挂点

- [对比学习](../concepts/contrastive.md)：给相关样本较高相似度，让它们在候选竞争中被找回来。图文配对是 CLIP 的监督来源。

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。

- [行为克隆](../concepts/bc.md)：直接监督观测到动作的映射，不必在每次更新中根据奖励搜索。

## 本篇行星与卫星

- [对比学习](r3m/contrastive.md) · 初读挂点
- [表征空间](r3m/representation.md) · 初读挂点
- [行为克隆](r3m/bc.md) · 初读挂点
- [本篇方法链路](r3m/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
