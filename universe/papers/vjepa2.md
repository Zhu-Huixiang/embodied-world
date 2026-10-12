# V-JEPA 2 星系

V-JEPA 2: Self-Supervised Video Models Enable Understanding, Prediction and Planning

**导读** · 世界模型与模型强化学习

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/vjepa2.md) · [原文](https://arxiv.org/abs/2506.09985) · [评分卡](../../leaderboard/papers/vjepa2/README.md)

masked video encoder/EMA目标先学表征；冻结编码器后训300M block-causal 动作 predictor，自回归预测未来 latent；MPC 最小化目标图 latent L1。

## 技术挂点

- [表征预测 JEPA](../concepts/jepa.md)：在表征空间预测目标而不是逐像素重建；防止表征坍缩仍需要相应设计。

- [动作条件动力学](../concepts/dynamics.md)：以当前状态和动作预测下一状态或分布，建立“做这个动作会发生什么”的计算接口。

- [模型预测控制 MPC](../concepts/mpc.md)：在模型里比较未来动作序列，执行开头一段，用新观测重算下一轮。

## 本篇行星与卫星

- [表征预测 JEPA](vjepa2/jepa.md) · 初读挂点
- [动作条件动力学](vjepa2/dynamics.md) · 初读挂点
- [模型预测控制 MPC](vjepa2/mpc.md) · 初读挂点
- [本篇方法链路](vjepa2/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
