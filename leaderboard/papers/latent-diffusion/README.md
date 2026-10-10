# High-Resolution Image Synthesis with Latent Diffusion Models

**Latent Diffusion** · CVPR 2022 · 本版排名 3 · 综合分 **95.8 / 100**

[解读导读](../../../library/latent-diffusion.md) · [Diffusion / Transformer 基础](../../../paper-map/README.md#track-diffusion-transformer) · [CVPR集锦](../../../venues/CVPR/README.md)

[原文](https://openaccess.thecvf.com/content/CVPR2022/html/Rombach_High-Resolution_Image_Synthesis_With_Latent_Diffusion_Models_CVPR_2022_paper.html) · [PDF](https://openaccess.thecvf.com/content/CVPR2022/papers/Rombach_High-Resolution_Image_Synthesis_With_Latent_Diffusion_Models_CVPR_2022_paper.pdf) · [阅读卡片](../../../library/latent-diffusion.md)

## 机制简析

先训练自动编码器，把高分辨率图像压成空间 latent；再在 latent 上训练扩散网络，最后解码为图像。文本或布局由条件编码器产生 token，并通过交叉注意力进入去噪网络。原文比较压缩程度、图像质量和计算成本，并评估文生图、修复与超分辨率。

带着这个问题读：为什么视频或图像模型常先压到 latent 空间，压缩省掉什么、又可能丢掉什么？

初读判断：表示压缩与生成训练拆得清楚，跨任务和压缩消融丰富，官方代码及权重可用；能帮助读者分析潜空间生成世界模型。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 94 | 20% |
| 实验与证据 | 94 | 20% |
| 学术影响 | 100 | 10% |
| 近期关注 | 100 | 5% |
| 复用价值 | 99 | 8% |
| 阅读价值 | 97 | 7% |

刊会依据：[CVPR 2022](../../../venues/CVPR/README.md)，正式出处见[出版/原文记录](https://openaccess.thecvf.com/content/CVPR2022/html/Rombach_High-Resolution_Image_Synthesis_With_Latent_Diffusion_Models_CVPR_2022_paper.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：正式刊会版本；OpenAlex题目：High-Resolution Image Synthesis with Latent Diffusion Models。累计被引 15913，2025–2026 被引 9591；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4312933868) · [文献计量条目](https://openalex.org/W4312933868)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
