# 注意力

按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。

自注意力在同一序列内读；交叉注意力读取另一组条件。

分类上层：[Transformer](transformer.md)。

继续拆：[因果序列建模](causal.md)。

## 哪些论文用到或讨论它

- [π₀](../papers/pi0.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss21/p010.html)
- [DiT](../papers/dit.md) · 机制导读 · [原文](https://openaccess.thecvf.com/content/ICCV2023/html/Peebles_Scalable_Diffusion_Models_with_Transformers_ICCV_2023_paper.html)
- [RT-1](../papers/rt1.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss19/p025.html)
- [PerAct](../papers/peract.md) · 机制导读 · [原文](https://proceedings.mlr.press/v205/shridhar23a.html)
- [RVT](../papers/rvt.md) · 机制导读 · [原文](https://proceedings.mlr.press/v229/goyal23a.html)
- [RVT-2](../papers/rvt2.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss20/p055.html)
- [VIMA](../papers/vima.md) · 机制导读 · [原文](https://proceedings.mlr.press/v202/jiang23b.html)
- [Transformer](../papers/attention.md) · 机制导读 · [原文](https://papers.nips.cc/paper/2017/hash/3f5ee243547dee91fbd053c1c4a845aa-Abstract.html)
- [ViT](../papers/vit.md) · 机制导读 · [原文](https://iclr.cc/virtual/2021/poster/3013)
- [SAM](../papers/sam.md) · 机制导读 · [原文](https://openaccess.thecvf.com/content/ICCV2023/html/Kirillov_Segment_Anything_ICCV_2023_paper.html)
- [SAM 2](../papers/sam2.md) · 机制导读 · [原文](https://openreview.net/forum?id=Ha6RTeWMd0)
- [Latent Diffusion](../papers/latent-diffusion.md) · 机制导读 · [原文](https://openaccess.thecvf.com/content/CVPR2022/html/Rombach_High-Resolution_Image_Synthesis_With_Latent_Diffusion_Models_CVPR_2022_paper.html)
- [Video Diffusion](../papers/video-diffusion.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2022/hash/39235c56aef13fb05a6adc95eb9d8d66-Abstract-Conference.html)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
