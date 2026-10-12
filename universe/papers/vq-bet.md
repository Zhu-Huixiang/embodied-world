# VQ-BeT 星系

Behavior Generation with Latent Actions

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/vq-bet.md) · [原文](https://proceedings.mlr.press/v235/lee24y.html) · [评分卡](../../leaderboard/papers/vq-bet/README.md)

第一阶段用残差向量量化编码器把连续动作或动作块压成分层码，解码器还原动作；第二阶段 Transformer 根据观测与可选目标预测这些离散码和修正量。一次前向生成替代扩散多步去噪，同时保留行为分布的多种模式。原文比较条件/无条件任务、仿真和真实长程操作，以及推理时延。

## 技术挂点

- [残差向量量化 RVQ](../concepts/rvq.md)：用第一层码近似向量，再用后续码近似剩余误差，最后把各层码相加重建。

- [离散编码与量化](../concepts/quantization.md)：把连续向量或信号映射到有限码。动作、视频潜变量与世界模型状态都可能采用这种表示，码本和训练目标各不相同。

- [因果序列建模](../concepts/causal.md)：通过遮罩只让位置读取允许的历史，避免训练时看到运行时不存在的未来。

## 本篇行星与卫星

- [残差向量量化 RVQ](vq-bet/rvq.md) · 初读挂点
- [离散编码与量化](vq-bet/quantization.md) · 初读挂点
- [因果序列建模](vq-bet/causal.md) · 初读挂点
- [本篇方法链路](vq-bet/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
