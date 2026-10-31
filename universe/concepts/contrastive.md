# 对比学习

给相关样本较高相似度，让它们在候选竞争中被找回来。图文配对是 CLIP 的监督来源。

CLIP 同批 N 对样本组成 N×N 相似度表，对角线是配对答案。

分类上层：[表征空间](representation.md)。

继续拆：[向量归一化](normalization.md) · [余弦相似度](cosine.md) · [交叉熵](cross-entropy.md)。

## 在完整解读里看计算与例子

- [CLIP：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#22-训练目标完整写一句话负担有点重)

## 哪些论文用到或讨论它

- [CLIPort](../papers/cliport.md) · 机制导读 · [原文](https://proceedings.mlr.press/v164/shridhar22a.html)
- [R3M](../papers/r3m.md) · 机制导读 · [原文](https://proceedings.mlr.press/v205/nair23a.html)
- [CLIP](../papers/clip.md) · 已精讲 · [原文](https://proceedings.mlr.press/v139/radford21a.html)
- [world2vec](../papers/world2vec.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.40637v1)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
