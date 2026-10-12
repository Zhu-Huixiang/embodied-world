# 提示模板集成

同一类别放进多种句子模板，编码后平均并归一化，减少单一表述对分类权重的影响。

CLIP 的模板集成先缓存类别向量，推理不必逐图重算所有文字。

分类上层：[零样本任务接口](zero-shot.md)。

## 在完整解读里看计算与例子

- [CLIP：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#25-使用一句话怎样变成分类器)

## 哪些论文用到或讨论它

- [CLIP](../papers/clip.md) · 已精讲 · [原文](https://proceedings.mlr.press/v139/radford21a.html)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
