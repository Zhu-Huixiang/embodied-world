# 视频时序生成

同时表达画面内容与时间变化，用历史与条件产生连续帧。

历史来自真值还是模型自己的输出，会影响滚动误差。

分类上层：[条件生成](generation.md)。

继续拆：[闭环滚动与历史偏移](rollout.md)。

## 哪些论文用到或讨论它

- [CoT-VLA](../papers/cot-vla.md) · 机制导读 · [原文](https://openaccess.thecvf.com/content/CVPR2025/html/Zhao_CoT-VLA_Visual_Chain-of-Thought_Reasoning_for_Vision-Language-Action_Models_CVPR_2025_paper.html)
- [DreamZero](../papers/dreamzero.md) · 机制导读 · [原文](https://arxiv.org/abs/2602.15922)
- [Cosmos Policy](../papers/cosmos-policy.md) · 机制导读 · [原文](https://openreview.net/forum?id=wPEIStHxYH)
- [VideoVLA](../papers/videovla.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2025/hash/89a3b655a8b68ae1c76b768152c9c19d-Abstract-Conference.html)
- [Diffusion Forcing](../papers/diffusion-forcing.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2024/hash/2aee1c4159e48407d68fe16ae8e6e49e-Abstract-Conference.html)
- [Self Forcing](../papers/self-forcing.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2025/hash/f4823f831af67a3ef15e41a85434422a-Abstract-Conference.html)
- [UniPi](../papers/unipi.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2023/hash/1d5b9233ad716a43be5c0d3023cb82d0-Abstract-Conference.html)
- [Video Diffusion](../papers/video-diffusion.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2022/hash/39235c56aef13fb05a6adc95eb9d8d66-Abstract-Conference.html)
- [Phenaki](../papers/phenaki.md) · 机制导读 · [原文](https://openreview.net/forum?id=vOEXS39nOF)
- [Ctrl-World](../papers/ctrl-world.md) · 机制导读 · [原文](https://proceedings.iclr.cc/paper_files/paper/2026/hash/0ae94013da7cd459402fd77874e09ee3-Abstract-Conference.html)
- [DreamTrue](../papers/dreamtrue.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.12468v1)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
