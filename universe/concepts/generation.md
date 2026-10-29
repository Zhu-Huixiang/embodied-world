# 条件生成

从一个条件生成多个可能输出，学习图像、视频或动作的分布而非只给一个均值。

条件可以是当前图、语言、目标状态或历史。

继续拆：[扩散去噪](diffusion.md) · [Flow Matching](flow.md) · [变分自编码器 VAE](vae.md) · [视频时序生成](video.md)。

## 在完整解读里看计算与例子

- [DDPM：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md#6-三个问题再落到机器人动作上)

## 哪些论文用到或讨论它

- [DDPM](../papers/ddpm.md) · 已精讲 · [原文](https://proceedings.neurips.cc/paper/2020/hash/4c5bcfec8584af0d967f1ab10179ca4b-Abstract.html)
- [DDIM](../papers/ddim.md) · 机制导读 · [原文](https://iclr.cc/virtual/2021/poster/2804)
- [EDM](../papers/edm.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2022/hash/a98846e9d9cc01cfb87eb694d946ce6b-Abstract-Conference.html)
- [Flow Matching](../papers/flow-matching.md) · 机制导读 · [原文](https://iclr.cc/virtual/2023/poster/11309)
- [Rectified Flow](../papers/rectified-flow.md) · 机制导读 · [原文](https://iclr.cc/virtual/2023/poster/11266)
- [Consistency Models](../papers/consistency-models.md) · 机制导读 · [原文](https://proceedings.mlr.press/v202/song23a.html)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
