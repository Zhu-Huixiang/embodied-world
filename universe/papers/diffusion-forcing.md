# Diffusion Forcing 星系

Diffusion Forcing: Next-token Prediction Meets Full-sequence Diffusion

**导读** · 视频与序列生成

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/diffusion-forcing.md) · [原文](https://proceedings.neurips.cc/paper_files/paper/2024/hash/2aee1c4159e48407d68fe16ae8e6e49e-Abstract-Conference.html) · [评分卡](../../leaderboard/papers/diffusion-forcing/README.md)

让序列各位置带不同噪声等级，把下一步预测与整段扩散连接，支持因果生成和引导。

## 技术挂点

- [扩散去噪](../concepts/diffusion.md)：训练网络从带噪对象估计噪声或干净目标，生成时从噪声开始迭代恢复样本。

- [因果序列建模](../concepts/causal.md)：通过遮罩只让位置读取允许的历史，避免训练时看到运行时不存在的未来。

- [视频时序生成](../concepts/video.md)：同时表达画面内容与时间变化，用历史与条件产生连续帧。

## 本篇行星与卫星

- [扩散去噪](diffusion-forcing/diffusion.md) · 初读挂点
- [因果序列建模](diffusion-forcing/causal.md) · 初读挂点
- [视频时序生成](diffusion-forcing/video.md) · 初读挂点
- [本篇方法链路](diffusion-forcing/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
