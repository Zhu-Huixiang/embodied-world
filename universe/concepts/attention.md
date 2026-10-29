# 注意力

按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。

自注意力在同一序列内读；交叉注意力读取另一组条件。

分类上层：[Transformer](transformer.md)。

继续拆：[因果序列建模](causal.md)。

## 在完整解读里看计算与例子

- [Transformer：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md#32-注意力qkv-分工不靠玄学)
- [DDPM：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md#36-打开-b-区u-net-里面怎样处理图像和时间)
- [Diffusion Policy：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/diffusion-policy-2303.04137/README.md#a-网络架构cnn-和-transformer-各干什么)
- [DINO：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dino-2104.14294/README.md#42-表示的新性质从找同类到找物体)
- [DiT：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dit-2212.09748/README.md#block-内部token-之间怎样互相看)
- [Latent Diffusion：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/latent-diffusion-2112.10752/README.md#33-条件机制文字如何进入图像的计算)
- [MAE：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/mae-2111.06377/README.md#32-b-区昂贵的编码器只招待真有内容的客人)
- [SAM：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam-2304.02643/README.md#33-c-区提示看图图也回头看提示)
- [ViT：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/vit-2010.11929/README.md#31-b-区注意力不是看见重点的黑箱)

## 哪些论文用到或讨论它

- [π₀](../papers/pi0.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss21/p010.html)
- [Diffusion Policy](../papers/diffusion-policy.md) · 已精讲 · [原文](https://www.roboticsproceedings.org/rss19/p026.html)
- [DiT](../papers/dit.md) · 已精讲 · [原文](https://openaccess.thecvf.com/content/ICCV2023/html/Peebles_Scalable_Diffusion_Models_with_Transformers_ICCV_2023_paper.html)
- [RT-1](../papers/rt1.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss19/p025.html)
- [PerAct](../papers/peract.md) · 机制导读 · [原文](https://proceedings.mlr.press/v205/shridhar23a.html)
- [RVT](../papers/rvt.md) · 机制导读 · [原文](https://proceedings.mlr.press/v229/goyal23a.html)
- [RVT-2](../papers/rvt2.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss20/p055.html)
- [VIMA](../papers/vima.md) · 机制导读 · [原文](https://proceedings.mlr.press/v202/jiang23b.html)
- [Transformer](../papers/attention.md) · 已精讲 · [原文](https://papers.nips.cc/paper/2017/hash/3f5ee243547dee91fbd053c1c4a845aa-Abstract.html)
- [ViT](../papers/vit.md) · 已精讲 · [原文](https://iclr.cc/virtual/2021/poster/3013)
- [DINO](../papers/dino.md) · 已精讲 · [原文](https://openaccess.thecvf.com/content/ICCV2021/html/Caron_Emerging_Properties_in_Self-Supervised_Vision_Transformers_ICCV_2021_paper.html)
- [MAE](../papers/mae.md) · 已精讲 · [原文](https://openaccess.thecvf.com/content/CVPR2022/html/He_Masked_Autoencoders_Are_Scalable_Vision_Learners_CVPR_2022_paper.html)
- [SAM](../papers/sam.md) · 已精讲 · [原文](https://openaccess.thecvf.com/content/ICCV2023/html/Kirillov_Segment_Anything_ICCV_2023_paper.html)
- [SAM 2](../papers/sam2.md) · 机制导读 · [原文](https://openreview.net/forum?id=Ha6RTeWMd0)
- [DDPM](../papers/ddpm.md) · 已精讲 · [原文](https://proceedings.neurips.cc/paper/2020/hash/4c5bcfec8584af0d967f1ab10179ca4b-Abstract.html)
- [Latent Diffusion](../papers/latent-diffusion.md) · 已精讲 · [原文](https://openaccess.thecvf.com/content/CVPR2022/html/Rombach_High-Resolution_Image_Synthesis_With_Latent_Diffusion_Models_CVPR_2022_paper.html)
- [Video Diffusion](../papers/video-diffusion.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2022/hash/39235c56aef13fb05a6adc95eb9d8d66-Abstract-Conference.html)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
