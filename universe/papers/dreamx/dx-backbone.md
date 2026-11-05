# 同一视频先验的编码与解码角色 · DreamX

Cosmos-Predict2.5 2B同时提供时空特征和生成先验。

编码器读取完整观察片段；解码器从首帧与latent重建未来。两者用独立rank16 LoRA，预训练骨干权重冻结。

继续拆：[5到29帧怎样变成潜视频](dx-video-latents.md) · [视频与动作共用条件而不互读](dx-decoder-mask.md)。

[本篇星系](../dreamx.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamx.md) · [原文依据](https://arxiv.org/pdf/2611.05377v1)
