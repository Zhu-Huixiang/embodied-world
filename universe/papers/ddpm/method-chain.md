# 本篇方法链路 · DDPM

正向过程逐步给数据加高斯噪声，训练时随机抽噪声时刻，让网络预测混入的噪声。反向生成从纯噪声开始，多步使用网络估计均值并采样，得到图像或换成动作序列后的条件样本。原文给出变分目标与简化去噪目标的联系，在 CIFAR-10 和 LSUN 评估图像生成质量。

正向过程逐步给数据加高斯噪声，训练时随机抽噪声时刻，让网络预测混入的噪声。反向生成从纯噪声开始，多步使用网络估计均值并采样，得到图像或换成动作序列后的条件样本。原文给出变分目标与简化去噪目标的联系，在 CIFAR-10 和 LSUN 评估图像生成质量。

[本篇星系](../ddpm.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/ddpm.md) · [原文依据](https://proceedings.neurips.cc/paper/2020/hash/4c5bcfec8584af0d967f1ab10179ca4b-Abstract.html)
