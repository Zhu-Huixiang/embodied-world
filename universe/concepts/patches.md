# 视觉 patch token

把图像切成块，展平并投影成向量，再加入位置信息。

CLIP B/32 的 224×224 图像得到 49 个图块，加 CLS 共 50 个视觉位置。

分类上层：[Transformer](transformer.md)。

## 在完整解读里看计算与例子

- [CLIP：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#23-模型两边各自干活最后才对答案)

## 哪些论文用到或讨论它

- [DiT](../papers/dit.md) · 机制导读 · [原文](https://openaccess.thecvf.com/content/ICCV2023/html/Peebles_Scalable_Diffusion_Models_with_Transformers_ICCV_2023_paper.html)
- [VC-1](../papers/vc1.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2023/hash/022ca1bed6b574b962c48a2856eb207b-Abstract-Conference.html)
- [ViT](../papers/vit.md) · 机制导读 · [原文](https://iclr.cc/virtual/2021/poster/3013)
- [CLIP](../papers/clip.md) · 已精讲 · [原文](https://proceedings.mlr.press/v139/radford21a.html)
- [DINOv2](../papers/dinov2.md) · 机制导读 · [原文](https://openreview.net/forum?id=a68SUt6zFt)
- [MAE](../papers/mae.md) · 机制导读 · [原文](https://openaccess.thecvf.com/content/CVPR2022/html/He_Masked_Autoencoders_Are_Scalable_Vision_Learners_CVPR_2022_paper.html)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
