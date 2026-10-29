# 分布偏移

测试场景的画风、视角、背景或对象组合发生变化，模型习惯的视觉线索随之改变。

CLIP Fig.7 横向匹配常规分数，再看偏移分布的高度。

分类上层：[表征空间](representation.md)。

## 在完整解读里看计算与例子

- [CLIP：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#34-换场景香蕉一变成素描就不认识了)
- [SAM 2：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam2-2408.00714/README.md#8-结论它给机器人补了哪块感知拼图)

## 哪些论文用到或讨论它

- [CLIP](../papers/clip.md) · 已精讲 · [原文](https://proceedings.mlr.press/v139/radford21a.html)
- [SAM 2](../papers/sam2.md) · 已精讲 · [原文](https://openreview.net/forum?id=Ha6RTeWMd0)
- [JAM](../papers/jam.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.37219v1)
- [TOPS](../papers/tops.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.36694v1)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
