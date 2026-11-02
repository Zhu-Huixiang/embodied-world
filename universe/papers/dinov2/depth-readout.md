# 有监督深度头把特征转成距离 · DINOv2

linear版本将CLS与patch拼接并上采样，用256个深度bin学习读出；DPT版本使用回归解码器。

Table11在冻结骨干上比较相同头类型。NYUd DPT .279对OpenCLIP .414 RMSE，目标仍来自深度标签。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#74-分割与深度)

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://arxiv.org/pdf/2304.07193v2)
