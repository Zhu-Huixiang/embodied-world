# Rectified Flow 星系

Flow Straight and Fast: Learning to Generate and Transfer Data with Rectified Flow

**导读** · Diffusion / Transformer 基础

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/rectified-flow.md) · [原文](https://iclr.cc/virtual/2023/poster/11266) · [评分卡](../../leaderboard/papers/rectified-flow/README.md)

从两个分布采样端点，用连接端点的线性插值训练速度场，让网络按当前位置估计路径速度。再用已有流生成配对数据重新训练，逐步减少轨迹弯曲，使粗时间步的数值积分更准确。原文给出传输代价性质，并在图像生成和域迁移中比较一步与多步效果。

## 技术挂点

- [Flow Matching](../concepts/flow.md)：给噪声到数据指定概率路径，回归沿路径的速度场；生成时数值积分这个场。

- [条件生成](../concepts/generation.md)：从一个条件生成多个可能输出，学习图像、视频或动作的分布而非只给一个均值。

## 本篇行星与卫星

- [Flow Matching](rectified-flow/flow.md) · 初读挂点
- [条件生成](rectified-flow/generation.md) · 初读挂点
- [本篇方法链路](rectified-flow/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
