# 扩散去噪

训练网络从带噪对象估计噪声或干净目标，生成时从噪声开始迭代恢复样本。

扩散采样步骤和机器人环境时间步是两种时间。

分类上层：[条件生成](generation.md)。

继续拆：[Diffusion Transformer](dit.md) · [一致性生成](consistency.md) · [去噪网络预条件化](preconditioning.md)。

## 在完整解读里看计算与例子

- [DDPM：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md#22-加噪公式里为什么还要把原图缩小)
- [Diffusion Policy：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/diffusion-policy-2303.04137/README.md#ii-diffusion-policy-formulation扩散对象变了)
- [DiT：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dit-2212.09748/README.md#31-先交代潜变量和噪声)
- [Latent Diffusion：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/latent-diffusion-2112.10752/README.md#32-潜空间扩散随机抽一道题学会整条去噪链)

## 哪些论文用到或讨论它

- [Diffusion Policy](../papers/diffusion-policy.md) · 已精讲 · [原文](https://www.roboticsproceedings.org/rss19/p026.html)
- [DP3](../papers/dp3.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss20/p067.html)
- [Consistency Policy](../papers/consistency-policy.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss20/p071.html)
- [Cosmos Policy](../papers/cosmos-policy.md) · 机制导读 · [原文](https://openreview.net/forum?id=wPEIStHxYH)
- [Diffusion Forcing](../papers/diffusion-forcing.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2024/hash/2aee1c4159e48407d68fe16ae8e6e49e-Abstract-Conference.html)
- [DiT](../papers/dit.md) · 已精讲 · [原文](https://openaccess.thecvf.com/content/ICCV2023/html/Peebles_Scalable_Diffusion_Models_with_Transformers_ICCV_2023_paper.html)
- [Octo](../papers/octo.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss20/p090.html)
- [UniPi](../papers/unipi.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2023/hash/1d5b9233ad716a43be5c0d3023cb82d0-Abstract-Conference.html)
- [Diffuser](../papers/diffuser.md) · 机制导读 · [原文](https://proceedings.mlr.press/v162/janner22a.html)
- [DDPM](../papers/ddpm.md) · 已精讲 · [原文](https://proceedings.neurips.cc/paper/2020/hash/4c5bcfec8584af0d967f1ab10179ca4b-Abstract.html)
- [DDIM](../papers/ddim.md) · 机制导读 · [原文](https://iclr.cc/virtual/2021/poster/2804)
- [Latent Diffusion](../papers/latent-diffusion.md) · 已精讲 · [原文](https://openaccess.thecvf.com/content/CVPR2022/html/Rombach_High-Resolution_Image_Synthesis_With_Latent_Diffusion_Models_CVPR_2022_paper.html)
- [EDM](../papers/edm.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2022/hash/a98846e9d9cc01cfb87eb694d946ce6b-Abstract-Conference.html)
- [Video Diffusion](../papers/video-diffusion.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2022/hash/39235c56aef13fb05a6adc95eb9d8d66-Abstract-Conference.html)
- [FLoRe](../papers/flore.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.35862v1)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
