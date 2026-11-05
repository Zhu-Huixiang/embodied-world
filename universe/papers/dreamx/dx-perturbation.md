# 扰动latent首先改变运动 · DreamX

8个挑选高运动clip、每clip两decoder seed，固定初始帧、噪声和采样设置。

alpha0.1/0.3/1与零query控制；零query平均相对运动比0.456。静态区域RGB变化更小，是选定片段上的敏感性分析，不保证所有latent完全无外观。

继续拆：[方向簇是聚合均值而非逐样本解耦](dx-centroids.md)。

[本篇星系](../dreamx.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamx.md) · [原文依据](https://arxiv.org/pdf/2611.05377v1)
