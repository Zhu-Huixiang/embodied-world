# FAST 星系

FAST: Efficient Action Tokenization for Vision-Language-Action Models

**导读** · 视觉语言动作模型 VLA

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/fast.md) · [原文](https://www.roboticsproceedings.org/rss21/p012.html) · [评分卡](../../leaderboard/papers/fast/README.md)

时间 DCT 提取动作频率系数，再量化和字节对编码，减少高频轨迹逐时刻离散产生的长序列。

## 技术挂点

- [DCT 频率系数](../concepts/dct.md)：把时间序列换到余弦频率基，低频系数描述缓慢变化，高频描述更快变化。

- [离散编码与量化](../concepts/quantization.md)：把连续向量或信号映射到有限码。动作、视频潜变量与世界模型状态都可能采用这种表示，码本和训练目标各不相同。

- [因果序列建模](../concepts/causal.md)：通过遮罩只让位置读取允许的历史，避免训练时看到运行时不存在的未来。

## 本篇行星与卫星

- [DCT 频率系数](fast/dct.md) · 初读挂点
- [离散编码与量化](fast/quantization.md) · 初读挂点
- [因果序列建模](fast/causal.md) · 初读挂点
- [本篇方法链路](fast/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
