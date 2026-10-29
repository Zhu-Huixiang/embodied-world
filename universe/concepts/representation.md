# 表征空间

把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。

512 维向量有 512 个实数，单个坐标通常没有预先指定的物理含义。

继续拆：[对比学习](contrastive.md) · [零样本任务接口](zero-shot.md) · [线性探测](linear-probe.md) · [分布偏移](shift.md) · [空间表示](spatial.md) · [遮蔽预测](masking.md) · [教师学生蒸馏](distill.md)。

## 在完整解读里看计算与例子

- [DINO：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dino-2104.14294/README.md#32-b-区骨干负责看投影头负责训练对齐)
- [3DGS：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/gaussian-splatting-2308.04079/README.md#41-b-区一个高斯不是一颗固定圆球)
- [Latent Diffusion：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/latent-diffusion-2112.10752/README.md#31-感知压缩先把画面装进一个靠谱的小空间)
- [MAE：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/mae-2111.06377/README.md#32-b-区昂贵的编码器只招待真有内容的客人)
- [MuZero：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md#33-atari-的观测到底怎样变成隐藏状态)
- [NeRF：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/nerf-2003.08934/README.md#32-mlp-里面到底走了几步)
- [RT-1：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md#51-a-区语言先改看法再决定做法)
- [SAM 2：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam2-2408.00714/README.md#41-a-区一张图先变成多尺度特征)
- [ViT：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/vit-2010.11929/README.md#31-cd-区cls-的代表发言权怎么来的)

## 哪些论文用到或讨论它

- [OpenVLA](../papers/openvla.md) · 机制导读 · [原文](https://proceedings.mlr.press/v270/kim25c.html)
- [ASE](../papers/ase.md) · 机制导读 · [原文](https://xbpeng.github.io/projects/ASE/)
- [RT-1](../papers/rt1.md) · 已精讲 · [原文](https://www.roboticsproceedings.org/rss19/p025.html)
- [PaLM-E](../papers/palm-e.md) · 机制导读 · [原文](https://proceedings.mlr.press/v202/driess23a.html)
- [R3M](../papers/r3m.md) · 机制导读 · [原文](https://proceedings.mlr.press/v205/nair23a.html)
- [VIP](../papers/vip.md) · 机制导读 · [原文](https://openreview.net/forum?id=YJ7o2wetJ2)
- [EfficientZero](../papers/efficientzero.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper/2021/hash/d5eca8dc3820cad9fe56a3bafda65ca1-Abstract.html)
- [MuZero](../papers/muzero.md) · 已精讲 · [原文](https://www.nature.com/articles/s41586-020-03051-4)
- [ViT](../papers/vit.md) · 已精讲 · [原文](https://iclr.cc/virtual/2021/poster/3013)
- [DINO](../papers/dino.md) · 已精讲 · [原文](https://openaccess.thecvf.com/content/ICCV2021/html/Caron_Emerging_Properties_in_Self-Supervised_Vision_Transformers_ICCV_2021_paper.html)
- [DINOv2](../papers/dinov2.md) · 机制导读 · [原文](https://openreview.net/forum?id=a68SUt6zFt)
- [MAE](../papers/mae.md) · 已精讲 · [原文](https://openaccess.thecvf.com/content/CVPR2022/html/He_Masked_Autoencoders_Are_Scalable_Vision_Learners_CVPR_2022_paper.html)
- [SAM 2](../papers/sam2.md) · 已精讲 · [原文](https://openreview.net/forum?id=Ha6RTeWMd0)
- [NeRF](../papers/nerf.md) · 已精讲 · [原文](https://link.springer.com/chapter/10.1007/978-3-030-58452-8_24)
- [3DGS](../papers/gaussian-splatting.md) · 已精讲 · [原文](https://dl.acm.org/doi/10.1145/3592433)
- [Latent Diffusion](../papers/latent-diffusion.md) · 已精讲 · [原文](https://openaccess.thecvf.com/content/CVPR2022/html/Rombach_High-Resolution_Image_Synthesis_With_Latent_Diffusion_Models_CVPR_2022_paper.html)
- [I-JEPA](../papers/i-jepa.md) · 机制导读 · [原文](https://openaccess.thecvf.com/content/CVPR2023/html/Assran_Self-Supervised_Learning_From_Images_With_a_Joint-Embedding_Predictive_Architecture_CVPR_2023_paper.html)
- [Dynamics Review](../papers/learned-dynamics-review.md) · 机制导读 · [原文](https://www.science.org/doi/10.1126/scirobotics.adt1497)
- [JAM](../papers/jam.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.37219v1)
- [VIOLA](../papers/viola.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.12435v1)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
