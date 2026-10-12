# PLaW-VLA 星系

PLaW-VLA: Predictive Latent World Modeling for Vision-Language-Action Policies

**导读** · 视频动作模型与视觉推理

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/plaw-vla.md) · [原文](https://arxiv.org/abs/2610.12285v1) · [评分卡](../../leaderboard/papers/plaw-vla/README.md)

预测面向任务的未来潜表示，再用结构化因果注意力让动作生成读取历史、任务和未来状态，减少无关像素重建。

## 技术挂点

- [表征预测 JEPA](../concepts/jepa.md)：在表征空间预测目标而不是逐像素重建；防止表征坍缩仍需要相应设计。

- [因果序列建模](../concepts/causal.md)：通过遮罩只让位置读取允许的历史，避免训练时看到运行时不存在的未来。

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

## 本篇行星与卫星

- [表征预测 JEPA](plaw-vla/jepa.md) · 初读挂点
- [因果序列建模](plaw-vla/causal.md) · 初读挂点
- [动作表示](plaw-vla/action.md) · 初读挂点
- [本篇方法链路](plaw-vla/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
