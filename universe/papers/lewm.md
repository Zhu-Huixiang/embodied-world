# LeWM 星系

LeWorldModel: Stable End-to-End Joint-Embedding Predictive Architecture from Pixels

**导读** · 世界模型与模型强化学习

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/lewm.md) · [原文](https://arxiv.org/abs/2603.19312v1) · [评分卡](../../leaderboard/papers/lewm/README.md)

ViT将每帧变成192维CLS表征；动作AdaLN条件的Transformer预测下个latent。MSE预测+SIGReg随机投影高斯正则共同训练，无EMA/stop-gradient/重建。部署用latent目标距离和CEM选动作，再MPC重规划。

## 技术挂点

- [表征预测 JEPA](../concepts/jepa.md)：在表征空间预测目标而不是逐像素重建；防止表征坍缩仍需要相应设计。

- [动作条件动力学](../concepts/dynamics.md)：以当前状态和动作预测下一状态或分布，建立“做这个动作会发生什么”的计算接口。

- [模型预测控制 MPC](../concepts/mpc.md)：在模型里比较未来动作序列，执行开头一段，用新观测重算下一轮。

## 本篇行星与卫星

- [表征预测 JEPA](lewm/jepa.md) · 初读挂点
- [动作条件动力学](lewm/dynamics.md) · 初读挂点
- [模型预测控制 MPC](lewm/mpc.md) · 初读挂点
- [本篇方法链路](lewm/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
