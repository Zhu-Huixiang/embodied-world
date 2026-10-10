# Denoising Diffusion Implicit Models

**解读导读** · ICLR 2021 · [Diffusion / Transformer 基础](../paper-map/README.md#track-diffusion-transformer)

研究范围：生成/表征基础，动作扩散与视频扩散的少步确定性采样。

[原文入口](https://iclr.cc/virtual/2021/poster/2804) · [原文 PDF](https://openreview.net/pdf?id=St1giarCHLP) · [作者项目 / 代码入口](https://github.com/ermongroup/ddim) · [作者与团队](../leaderboard/origins/papers/ddim.md)

ICLR 2021 正式论文；同一 DDPM 训练目标与不同推理路径分开解释。

## 先看它做了什么

构造共享相同加噪边缘分布的非马尔可夫过程，使训练仍然使用 DDPM 的噪声预测目标。推理则选择子时间序列和相应更新规则，确定性情形可以少步从噪声映射到数据。原文比较不同步数的生成速度、质量、插值和重建，揭示采样器改动无需等同于重新训练模型。

## 带着什么问题读

**去噪训练目标不变，为什么推理时能跳步，延迟与样本质量该怎样交换？**

## 为什么值得继续读

扩散策略的在线延迟问题需要理解采样器与训练目标的区别；DDIM 是这个分离的经典算法，官方复现实现在多个扩散代码库可使用。

证据入口：采样与训练的解耦具有明确算法价值，速度质量曲线和重建实验具体，公开实现很适合具身推理教程。

具身关联：扩散策略的在线延迟问题需要理解采样器与训练目标的区别；DDIM 是这个分离的经典算法，官方复现实现在多个扩散代码库可使用。

经典保留理由：ICLR 2021 早于 2021-10-10；作为少步扩散采样经典，直接服务机器人动作实时推理与视频预测的延迟分析。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/ddim/README.md) · [ICLR集锦](../venues/ICLR/README.md) · [地图方向](../paper-map/README.md#track-diffusion-transformer) · [首页](../README.md)

元数据核对：2026-10-10。
