# 可优化三维高斯 · 3DGS

中心与协方差决定空间权重形状。

μ为3维，Σ为3×3；高斯没有硬边界，离中心越远权重越小。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/gaussian-splatting-2308.04079/README.md#41-b-区一个高斯不是一颗固定圆球)

继续拆：[各向异性尺度旋转](anisotropic.md) · [投影协方差](projection.md) · [球谐方向颜色](sh.md)。

[本篇星系](../gaussian-splatting.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/gaussian-splatting-2308.04079/README.md) · [原文依据](https://arxiv.org/abs/2308.04079v1)
