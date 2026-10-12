# LeWAM 星系

LeWAM: A JEPA World Action Model with Diffusion-Steering-Based MPC

**导读** · 世界动作模型

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/lewam.md) · [原文](https://arxiv.org/abs/2610.12407v1) · [评分卡](../../leaderboard/papers/lewam/README.md)

在不重建图像的 JEPA 表征上联合学前向、后向、逆动力学和策略；MPC 在策略噪声空间采样，降低规划钻动力学模型空子的机会。

## 技术挂点

- [表征预测 JEPA](../concepts/jepa.md)：在表征空间预测目标而不是逐像素重建；防止表征坍缩仍需要相应设计。

- [动作条件动力学](../concepts/dynamics.md)：以当前状态和动作预测下一状态或分布，建立“做这个动作会发生什么”的计算接口。

- [逆动力学](../concepts/inverse.md)：从状态变化或相邻画面推回可能的动作，给视频计划连接环境专用执行接口。

- [模型预测控制 MPC](../concepts/mpc.md)：在模型里比较未来动作序列，执行开头一段，用新观测重算下一轮。

## 本篇行星与卫星

- [表征预测 JEPA](lewam/jepa.md) · 初读挂点
- [动作条件动力学](lewam/dynamics.md) · 初读挂点
- [逆动力学](lewam/inverse.md) · 初读挂点
- [模型预测控制 MPC](lewam/mpc.md) · 初读挂点
- [本篇方法链路](lewam/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
