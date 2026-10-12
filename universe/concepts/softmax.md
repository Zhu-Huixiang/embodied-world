# softmax 与温度

对候选分数取指数后归一化为总和为 1 的概率。温度控制分差如何影响概率。

温度改变概率集中程度；候选集合也会改变概率分母。

分类上层：[交叉熵](cross-entropy.md)。

## 在完整解读里看计算与例子

- [CLIP：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#22-训练目标完整写一句话负担有点重)

## 哪些论文用到或讨论它

- [CLIP](../papers/clip.md) · 已精讲 · [原文](https://proceedings.mlr.press/v139/radford21a.html)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
