# 前向透明度合成 · 3DGS

从近到远按剩余透射率累积颜色。

前层越不透明，留给后层的权重越少；红0.6与蓝0.5示例得到(0.6,0,0.2)。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/gaussian-splatting-2308.04079/README.md#43-颜色随方向变遮挡按顺序算)

[本篇星系](../gaussian-splatting.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/gaussian-splatting-2308.04079/README.md) · [原文依据](https://arxiv.org/abs/2308.04079v1)
