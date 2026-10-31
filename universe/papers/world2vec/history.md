# 三帧历史补充速度信息 · world2vec

单帧位置不能决定速度，用H=3的短历史编码。

每帧64×64 RGB由小ViT编码，再经拼接历史的MLP得到z；潜宽按实验变化，d=32结构的263k参数不代表所有表格行精确参数数。

继续拆：[潜向量场与Euler残差](euler.md) · [随机动作视觉数据与切分](dataset.md)。

[本篇星系](../world2vec.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/world2vec.md) · [原文依据](https://arxiv.org/pdf/2610.40637v1)
