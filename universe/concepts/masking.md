# 遮蔽预测

隐藏部分输入，训练模型恢复像素、token 或表征。恢复什么决定监督重点。

MAE 恢复像素，JEPA 类方法预测表征。

分类上层：[表征空间](representation.md)。

继续拆：[表征预测 JEPA](jepa.md)。

## 在完整解读里看计算与例子

- [MAE：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/mae-2111.06377/README.md#31-a-区随机藏起来位置仍然留着)

## 哪些论文用到或讨论它

- [VC-1](../papers/vc1.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2023/hash/022ca1bed6b574b962c48a2856eb207b-Abstract-Conference.html)
- [MaskedMimic](../papers/maskedmimic.md) · 机制导读 · [原文](https://dl.acm.org/doi/10.1145/3687951)
- [MAE](../papers/mae.md) · 已精讲 · [原文](https://openaccess.thecvf.com/content/CVPR2022/html/He_Masked_Autoencoders_Are_Scalable_Vision_Learners_CVPR_2022_paper.html)
- [Phenaki](../papers/phenaki.md) · 机制导读 · [原文](https://openreview.net/forum?id=vOEXS39nOF)
- [I-JEPA](../papers/i-jepa.md) · 机制导读 · [原文](https://openaccess.thecvf.com/content/CVPR2023/html/Assran_Self-Supervised_Learning_From_Images_With_a_Joint-Embedding_Predictive_Architecture_CVPR_2023_paper.html)
- [HOVER](../papers/hover.md) · 机制导读 · [原文](https://hover-versatile-humanoid.github.io/)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
