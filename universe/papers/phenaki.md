# Phenaki 星系

Phenaki: Variable Length Video Generation From Open Domain Textual Descriptions

**导读** · 视频与序列生成

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/phenaki.md) · [原文](https://openreview.net/forum?id=vOEXS39nOF) · [评分卡](../../leaderboard/papers/phenaki/README.md)

C-ViViT 用因果时间注意力把可变长度视频压成离散 token，兼顾空间与时间压缩。文本特征条件化双向掩码 Transformer，逐轮补齐视频 token 后再解码；继续生成时复用已有上下文。原文检查视频压缩、时序质量和图文/视频联合训练，并展示随文本故事变化的长视频。

## 技术挂点

- [视频时序生成](../concepts/video.md)：同时表达画面内容与时间变化，用历史与条件产生连续帧。

- [离散编码与量化](../concepts/quantization.md)：把连续向量或信号映射到有限码。动作、视频潜变量与世界模型状态都可能采用这种表示，码本和训练目标各不相同。

- [遮蔽预测](../concepts/masking.md)：隐藏部分输入，训练模型恢复像素、token 或表征。恢复什么决定监督重点。

## 本篇行星与卫星

- [视频时序生成](phenaki/video.md) · 初读挂点
- [离散编码与量化](phenaki/quantization.md) · 初读挂点
- [遮蔽预测](phenaki/masking.md) · 初读挂点
- [本篇方法链路](phenaki/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
