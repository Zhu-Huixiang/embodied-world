# 交叉注意力的两种方向 · SAM

query一侧被更新，key/value一侧被读取。

先让输出token读取4096个图像位置，再把提示约束写回空间特征。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam-2304.02643/README.md#33-c-区提示看图图也回头看提示)

[本篇星系](../sam.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam-2304.02643/README.md) · [原文依据](https://arxiv.org/abs/2304.02643v1)
