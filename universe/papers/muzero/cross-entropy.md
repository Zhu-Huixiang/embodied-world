# 交叉熵 · MuZero

用目标概率分布加权预测概率的负对数，再求和。目标集中在一个正确类别时，就是该类别的负对数概率。

CLIP用配对图文的位置作目标；DINOv2用教师给出的软分布监督学生。目标分布自身有熵，预测对齐后交叉熵也未必为零。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md#36-损失函数三份作业一起改hgf)

[跨论文技术入口](../../concepts/cross-entropy.md)

[本篇星系](../muzero.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md) · [原文依据](https://www.nature.com/articles/s41586-020-03051-4)
