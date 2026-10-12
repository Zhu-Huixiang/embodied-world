# Self Forcing 星系

Self Forcing: Bridging the Train-Test Gap in Autoregressive Video Diffusion

**导读** · 视频与序列生成

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/self-forcing.md) · [原文](https://proceedings.neurips.cc/paper_files/paper/2025/hash/f4823f831af67a3ef15e41a85434422a-Abstract-Conference.html) · [评分卡](../../leaderboard/papers/self-forcing/README.md)

使用模型自己的历史滚动来训练自回归视频生成，减少教师历史与部署历史的分布差异。

## 技术挂点

- [视频时序生成](../concepts/video.md)：同时表达画面内容与时间变化，用历史与条件产生连续帧。

- [因果序列建模](../concepts/causal.md)：通过遮罩只让位置读取允许的历史，避免训练时看到运行时不存在的未来。

- [闭环滚动与历史偏移](../concepts/rollout.md)：重复预测、执行或生成，把新观测或模型历史接回后续计算。

## 本篇行星与卫星

- [视频时序生成](self-forcing/video.md) · 初读挂点
- [因果序列建模](self-forcing/causal.md) · 初读挂点
- [闭环滚动与历史偏移](self-forcing/rollout.md) · 初读挂点
- [本篇方法链路](self-forcing/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
