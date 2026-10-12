# VIP 星系

VIP: Towards Universal Visual Reward and Representation via Value-Implicit Pre-Training

**导读** · 具身感知与场景表示

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/vip.md) · [原文](https://openreview.net/forum?id=YJ7o2wetJ2) · [评分卡](../../leaderboard/papers/vip/README.md)

把无动作视频看成目标条件价值学习，再从离线 RL 的对偶目标导出仅需要画面序列的预训练损失。价值隐式地由当前图像与目标图像的嵌入距离表达，因而距离变化能提供稠密视觉奖励。原文检验轨迹优化、在线 RL 与少量真实轨迹的离线 RL，强调表征和奖励同时影响控制。

## 技术挂点

- [价值估计与校准](../concepts/value.md)：估计未来累积收益，再用保守、分位或参考价值等约束减少误导。

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。

- [强化学习](../concepts/rl.md)：通过奖励和值评估改进策略，研究动作如何改变长期回报。

## 本篇行星与卫星

- [价值估计与校准](vip/value.md) · 初读挂点
- [表征空间](vip/representation.md) · 初读挂点
- [强化学习](vip/rl.md) · 初读挂点
- [本篇方法链路](vip/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
