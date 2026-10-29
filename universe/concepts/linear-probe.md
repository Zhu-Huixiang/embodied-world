# 线性探测

冻结编码器，用带标签的下游样本训练线性预测头，以检查特征本身是否容易迁移。

要分清读取投影前特征还是归一化图文向量。

分类上层：[表征空间](representation.md)。

## 在完整解读里看计算与例子

- [CLIP：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#33-表征换个分类头才能单独看视觉底子)
- [DINO：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dino-2104.14294/README.md#41-最普通的分类读出方式却要分清)
- [MAE：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/mae-2111.06377/README.md#43-部分微调线性探测没看见的能力)
- [ViT：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/vit-2010.11929/README.md#43-数据需求大模型吃瘪那张图才是论文的转折)

## 哪些论文用到或讨论它

- [ViT](../papers/vit.md) · 已精讲 · [原文](https://iclr.cc/virtual/2021/poster/3013)
- [CLIP](../papers/clip.md) · 已精讲 · [原文](https://proceedings.mlr.press/v139/radford21a.html)
- [DINO](../papers/dino.md) · 已精讲 · [原文](https://openaccess.thecvf.com/content/ICCV2021/html/Caron_Emerging_Properties_in_Self-Supervised_Vision_Transformers_ICCV_2021_paper.html)
- [MAE](../papers/mae.md) · 已精讲 · [原文](https://openaccess.thecvf.com/content/CVPR2022/html/He_Masked_Autoencoders_Are_Scalable_Vision_Learners_CVPR_2022_paper.html)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
