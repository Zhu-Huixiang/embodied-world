# Cosmos Policy 星系

Cosmos Policy: Fine-Tuning Video Models for Visuomotor Control and Planning

**导读** · 世界动作模型

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/cosmos-policy.md) · [原文](https://openreview.net/forum?id=wPEIStHxYH) · [评分卡](../../leaderboard/papers/cosmos-policy/README.md)

微调视频基础模型，把动作、未来视觉状态和规划信号放进共同生成过程。

## 技术挂点

- [世界动作联合建模](../concepts/wam.md)：把未来状态或视频与动作放进联合条件生成过程，让视觉动态和行动相互约束。

- [视频时序生成](../concepts/video.md)：同时表达画面内容与时间变化，用历史与条件产生连续帧。

- [扩散去噪](../concepts/diffusion.md)：训练网络从带噪对象估计噪声或干净目标，生成时从噪声开始迭代恢复样本。

## 本篇行星与卫星

- [世界动作联合建模](cosmos-policy/wam.md) · 初读挂点
- [视频时序生成](cosmos-policy/video.md) · 初读挂点
- [扩散去噪](cosmos-policy/diffusion.md) · 初读挂点
- [本篇方法链路](cosmos-policy/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
