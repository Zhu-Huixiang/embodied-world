# Transformer

用注意力交换 token 信息，再逐位置加工。token 可以来自字词、图像块、状态或动作。

不同遮罩决定哪些位置能读到哪些信息。

继续拆：[注意力](attention.md) · [视觉 patch token](patches.md)。

## 在完整解读里看计算与例子

- [ACT / ALOHA：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/act-2304.13705/README.md#44-transformer四台相机怎样变成10014)
- [Transformer：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md#31-编码器与解码器两列各六层)
- [RT-1：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md#51-c-区transformer-输出的是动作档位)
- [SAM 2：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam2-2408.00714/README.md#43-c-区点击候选掩码与它现在不在)

## 哪些论文用到或讨论它

- [ACT / ALOHA](../papers/act.md) · 已精讲 · [原文](https://www.roboticsproceedings.org/rss19/p016.html)
- [RT-1](../papers/rt1.md) · 已精讲 · [原文](https://www.roboticsproceedings.org/rss19/p025.html)
- [Transformer](../papers/attention.md) · 已精讲 · [原文](https://papers.nips.cc/paper/2017/hash/3f5ee243547dee91fbd053c1c4a845aa-Abstract.html)
- [SAM 2](../papers/sam2.md) · 已精讲 · [原文](https://openreview.net/forum?id=Ha6RTeWMd0)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
