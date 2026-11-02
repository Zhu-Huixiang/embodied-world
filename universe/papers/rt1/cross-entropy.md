# 交叉熵 · RT-1

用目标概率分布加权预测概率的负对数，再求和。目标集中在一个正确类别时，就是该类别的负对数概率。

CLIP用配对图文的位置作目标；DINOv2用教师给出的软分布监督学生。目标分布自身有熵，预测对齐后交叉熵也未必为零。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md#52-d-区监督的答案就是人类当时选的动作)

[跨论文技术入口](../../concepts/cross-entropy.md)

[本篇星系](../rt1.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md) · [原文依据](https://www.roboticsproceedings.org/rss19/p025.html)
