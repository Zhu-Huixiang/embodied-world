# 线性探测

冻结编码器，用带标签的下游样本训练线性预测头，以检查特征本身是否容易迁移。

要分清读取投影前特征还是归一化图文向量。

分类上层：[表征空间](representation.md)。

## 在完整解读里看计算与例子

- [CLIP：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#33-表征换个分类头才能单独看视觉底子)

## 哪些论文用到或讨论它

- [CLIP](../papers/clip.md) · 已精讲 · [原文](https://proceedings.mlr.press/v139/radford21a.html)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
