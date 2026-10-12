# 本篇方法链路 · Phenaki

C-ViViT 用因果时间注意力把可变长度视频压成离散 token，兼顾空间与时间压缩。文本特征条件化双向掩码 Transformer，逐轮补齐视频 token 后再解码；继续生成时复用已有上下文。原文检查视频压缩、时序质量和图文/视频联合训练，并展示随文本故事变化的长视频。

C-ViViT 用因果时间注意力把可变长度视频压成离散 token，兼顾空间与时间压缩。文本特征条件化双向掩码 Transformer，逐轮补齐视频 token 后再解码；继续生成时复用已有上下文。原文检查视频压缩、时序质量和图文/视频联合训练，并展示随文本故事变化的长视频。

[本篇星系](../phenaki.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/phenaki.md) · [原文依据](https://openreview.net/forum?id=vOEXS39nOF)
