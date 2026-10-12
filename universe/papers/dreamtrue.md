# DreamTrue 星系

DreamTrue: Action-Faithful Robot World Model with Counterfactual Post-Training

**导读** · 世界模型与模型强化学习

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamtrue.md) · [原文](https://arxiv.org/abs/2610.12468v1) · [评分卡](../../leaderboard/papers/dreamtrue/README.md)

将动作轨迹渲染进图像条件并校准，改变轨迹生成反事实未来，再用人标视频缺陷训练奖励模型指导后训练。

## 技术挂点

- [动作条件动力学](../concepts/dynamics.md)：以当前状态和动作预测下一状态或分布，建立“做这个动作会发生什么”的计算接口。

- [视频时序生成](../concepts/video.md)：同时表达画面内容与时间变化，用历史与条件产生连续帧。

- [价值估计与校准](../concepts/value.md)：估计未来累积收益，再用保守、分位或参考价值等约束减少误导。

## 本篇行星与卫星

- [动作条件动力学](dreamtrue/dynamics.md) · 初读挂点
- [视频时序生成](dreamtrue/video.md) · 初读挂点
- [价值估计与校准](dreamtrue/value.md) · 初读挂点
- [本篇方法链路](dreamtrue/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
