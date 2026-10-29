# 零样本任务接口

不用目标数据集训练样本拟合分类头，而用任务描述等已有信息直接构造预测接口。

CLIP 将类别句子编码为权重，新图与它们比较。

分类上层：[表征空间](representation.md)。

继续拆：[提示模板集成](prompt-ensemble.md)。

## 在完整解读里看计算与例子

- [CLIP：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#25-使用一句话怎样变成分类器)
- [SAM：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam-2304.02643/README.md#61-先看单点再看多点)

## 哪些论文用到或讨论它

- [SayCan](../papers/saycan.md) · 机制导读 · [原文](https://proceedings.mlr.press/v205/ichter23a.html)
- [CLIP](../papers/clip.md) · 已精讲 · [原文](https://proceedings.mlr.press/v139/radford21a.html)
- [SAM](../papers/sam.md) · 已精讲 · [原文](https://openaccess.thecvf.com/content/ICCV2023/html/Kirillov_Segment_Anything_ICCV_2023_paper.html)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
