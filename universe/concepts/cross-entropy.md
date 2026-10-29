# 交叉熵

正确候选的负对数概率。正确项概率越小，损失越大，梯度会推动正确分数上升。

CLIP 对行和列分别计算平均交叉熵，再平均两个方向。

分类上层：[对比学习](contrastive.md)。

继续拆：[softmax 与温度](softmax.md)。

## 在完整解读里看计算与例子

- [Transformer：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md#5-训练答案右移未来遮住)
- [CLIP：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#22-训练目标完整写一句话负担有点重)
- [DINO：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dino-2104.14294/README.md#33-c-区把分数变分布再跨视图对答案)
- [MuZero：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md#36-损失函数三份作业一起改hgf)
- [RT-1：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md#52-d-区监督的答案就是人类当时选的动作)
- [SAM 2：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam2-2408.00714/README.md#45-e-区训练时怎样教它别跟丢)

## 哪些论文用到或讨论它

- [RT-1](../papers/rt1.md) · 已精讲 · [原文](https://www.roboticsproceedings.org/rss19/p025.html)
- [MuZero](../papers/muzero.md) · 已精讲 · [原文](https://www.nature.com/articles/s41586-020-03051-4)
- [Transformer](../papers/attention.md) · 已精讲 · [原文](https://papers.nips.cc/paper/2017/hash/3f5ee243547dee91fbd053c1c4a845aa-Abstract.html)
- [CLIP](../papers/clip.md) · 已精讲 · [原文](https://proceedings.mlr.press/v139/radford21a.html)
- [DINO](../papers/dino.md) · 已精讲 · [原文](https://openaccess.thecvf.com/content/ICCV2021/html/Caron_Emerging_Properties_in_Self-Supervised_Vision_Transformers_ICCV_2021_paper.html)
- [SAM 2](../papers/sam2.md) · 已精讲 · [原文](https://openreview.net/forum?id=Ha6RTeWMd0)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
