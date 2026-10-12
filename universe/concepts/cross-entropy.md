# 交叉熵

正确候选的负对数概率。正确项概率越小，损失越大，梯度会推动正确分数上升。

CLIP 对行和列分别计算平均交叉熵，再平均两个方向。

分类上层：[对比学习](contrastive.md)。

继续拆：[softmax 与温度](softmax.md)。

## 在完整解读里看计算与例子

- [CLIP：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#22-训练目标完整写一句话负担有点重)

## 哪些论文用到或讨论它

- [CLIP](../papers/clip.md) · 已精讲 · [原文](https://proceedings.mlr.press/v139/radford21a.html)
- [DINO](../papers/dino.md) · 机制导读 · [原文](https://openaccess.thecvf.com/content/ICCV2021/html/Caron_Emerging_Properties_in_Self-Supervised_Vision_Transformers_ICCV_2021_paper.html)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
