# 表征预测 JEPA

在表征空间预测目标而不是逐像素重建；防止表征坍缩仍需要相应设计。

不同论文的 EMA、stop-gradient 或正则方案不能互相借用。

分类上层：[遮蔽预测](masking.md)。

## 哪些论文用到或讨论它

- [I-JEPA](../papers/i-jepa.md) · 机制导读 · [原文](https://openaccess.thecvf.com/content/CVPR2023/html/Assran_Self-Supervised_Learning_From_Images_With_a_Joint-Embedding_Predictive_Architecture_CVPR_2023_paper.html)
- [LeWM](../papers/lewm.md) · 机制导读 · [原文](https://arxiv.org/abs/2603.19312v1)
- [V-JEPA 2](../papers/vjepa2.md) · 机制导读 · [原文](https://arxiv.org/abs/2506.09985)
- [JAM](../papers/jam.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.37219v1)
- [LeWAM](../papers/lewam.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.12407v1)
- [PLaW-VLA](../papers/plaw-vla.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.12285v1)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
