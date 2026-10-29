# softmax 与温度

对候选分数取指数后归一化为总和为 1 的概率。温度控制分差如何影响概率。

温度改变概率集中程度；候选集合也会改变概率分母。

分类上层：[交叉熵](cross-entropy.md)。

## 在完整解读里看计算与例子

- [Transformer：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md#32-注意力qkv-分工不靠玄学)
- [CLIP：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#22-训练目标完整写一句话负担有点重)
- [DINO：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dino-2104.14294/README.md#33-c-区把分数变分布再跨视图对答案)

## 哪些论文用到或讨论它

- [Transformer](../papers/attention.md) · 已精讲 · [原文](https://papers.nips.cc/paper/2017/hash/3f5ee243547dee91fbd053c1c4a845aa-Abstract.html)
- [CLIP](../papers/clip.md) · 已精讲 · [原文](https://proceedings.mlr.press/v139/radford21a.html)
- [DINO](../papers/dino.md) · 已精讲 · [原文](https://openaccess.thecvf.com/content/ICCV2021/html/Caron_Emerging_Properties_in_Self-Supervised_Vision_Transformers_ICCV_2021_paper.html)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
