# DreamZero 星系

World Action Models are Zero-shot Policies

**导读** · 世界动作模型

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamzero.md) · [原文](https://arxiv.org/abs/2602.15922) · [评分卡](../../leaderboard/papers/dreamzero/README.md)

联合建模未来视频与动作，将大规模视觉动态先验用于未见任务的闭环策略。

## 技术挂点

- [世界动作联合建模](../concepts/wam.md)：把未来状态或视频与动作放进联合条件生成过程，让视觉动态和行动相互约束。

- [视频时序生成](../concepts/video.md)：同时表达画面内容与时间变化，用历史与条件产生连续帧。

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

## 本篇行星与卫星

- [世界动作联合建模](dreamzero/wam.md) · 初读挂点
- [视频时序生成](dreamzero/video.md) · 初读挂点
- [动作表示](dreamzero/action.md) · 初读挂点
- [本篇方法链路](dreamzero/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
