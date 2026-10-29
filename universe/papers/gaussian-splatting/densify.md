# 自适应密度控制 · 3DGS

梯度和尺度决定何处增加高斯。

每100步处理，高位置梯度提示需要调整；小图元欠覆盖clone，大图元撑细节split。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/gaussian-splatting-2308.04079/README.md#52-密度控制不是哪里不清楚都狂撒点)

继续拆：[复制小高斯](clone.md) · [拆分大高斯](split.md) · [修剪和透明度重置](prune.md)。

[本篇星系](../gaussian-splatting.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/gaussian-splatting-2308.04079/README.md) · [原文依据](https://arxiv.org/abs/2308.04079v1)
