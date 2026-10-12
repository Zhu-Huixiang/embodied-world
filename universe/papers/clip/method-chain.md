# 本篇方法链路 · CLIP

图像编码器和文本编码器分别输出向量，经投影与归一化后计算一个批次中全部图文配对的相似度矩阵。对称交叉熵把真实配对拉近，把批内错配分开；测试时用文本描述生成类别向量，从而做零样本分类。原文在三十余个视觉数据集测试迁移，CLIPort 再将其语义特征与空间操作分支融合。

图像编码器和文本编码器分别输出向量，经投影与归一化后计算一个批次中全部图文配对的相似度矩阵。对称交叉熵把真实配对拉近，把批内错配分开；测试时用文本描述生成类别向量，从而做零样本分类。原文在三十余个视觉数据集测试迁移，CLIPort 再将其语义特征与空间操作分支融合。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#2-方法把图和文字放到同一张坐标纸上)

[本篇星系](../clip.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md) · [原文依据](https://proceedings.mlr.press/v139/radford21a.html)
