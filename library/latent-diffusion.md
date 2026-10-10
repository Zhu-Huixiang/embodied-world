# High-Resolution Image Synthesis with Latent Diffusion Models

**解读导读** · CVPR 2022 · [Diffusion / Transformer 基础](../paper-map/README.md#track-diffusion-transformer)

研究范围：生成/表征基础，潜空间视频世界模型与条件生成的编码/解码链路。

[原文入口](https://openaccess.thecvf.com/content/CVPR2022/html/Rombach_High-Resolution_Image_Synthesis_With_Latent_Diffusion_Models_CVPR_2022_paper.html) · [原文 PDF](https://openaccess.thecvf.com/content/CVPR2022/papers/Rombach_High-Resolution_Image_Synthesis_With_Latent_Diffusion_Models_CVPR_2022_paper.pdf) · [作者项目 / 代码入口](https://github.com/CompVis/latent-diffusion) · [作者与团队](../leaderboard/origins/papers/latent-diffusion.md)

CVPR 2022 原始 LDM；后续视频模型与机器人方法使用的具体编码器和条件接口需逐篇再核。

## 先看它做了什么

先训练自动编码器，把高分辨率图像压成空间 latent；再在 latent 上训练扩散网络，最后解码为图像。文本或布局由条件编码器产生 token，并通过交叉注意力进入去噪网络。原文比较压缩程度、图像质量和计算成本，并评估文生图、修复与超分辨率。

## 带着什么问题读

**为什么视频或图像模型常先压到 latent 空间，压缩省掉什么、又可能丢掉什么？**

## 为什么值得继续读

压缩表示中去噪与跨注意力条件化是现代潜空间视频/世界生成的常见构件；这篇把表示代价和生成代价拆开，值得作为后续阅读基础。

证据入口：表示压缩与生成训练拆得清楚，跨任务和压缩消融丰富，官方代码及权重可用；能帮助读者分析潜空间生成世界模型。

具身关联：压缩表示中去噪与跨注意力条件化是现代潜空间视频/世界生成的常见构件；这篇把表示代价和生成代价拆开，值得作为后续阅读基础。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/latent-diffusion/README.md) · [CVPR集锦](../venues/CVPR/README.md) · [地图方向](../paper-map/README.md#track-diffusion-transformer) · [首页](../README.md)

元数据核对：2026-10-10。
