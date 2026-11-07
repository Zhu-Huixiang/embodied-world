# 固定协方差高斯策略 · DeepMimic

MLP输出状态相关动作均值，固定对角协方差提供采样分布。

两隐藏层1024/512且用ReLU，最后线性输出；探索噪声作用于动作。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md#52-网络)

继续拆：[标量value网络](scalar-critic.md) · [高度图特征支路](heightmap-cnn.md)。

[本篇星系](../deepmimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md) · [原文依据](https://xbpeng.github.io/projects/DeepMimic/DeepMimic_2018.pdf)
