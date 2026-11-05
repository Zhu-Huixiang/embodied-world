# 5到29帧怎样变成潜视频 · DreamX

因果视频自编码器将输入压成2到8个潜帧，首个潜帧只含初始图像。

480×640视频以4帧为增量选5–29帧；随后patchify并进入视频Transformer。输入视频、VAE潜帧和latent-action token是三种不同粒度。

继续拆：[每个潜帧只读出四个查询](dx-queries.md)。

[本篇星系](../dreamx.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamx.md) · [原文依据](https://arxiv.org/pdf/2611.05377v1)
