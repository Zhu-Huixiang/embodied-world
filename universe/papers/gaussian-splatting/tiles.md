# 分块复制与排序 · 3DGS

把图元分配到它覆盖的16×16像素tile。

对每个tile的可见图元按tileID和深度key组织排序，便于GPU并行处理像素。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/gaussian-splatting-2308.04079/README.md#6-光栅化gpu-实际忙的是什么)

继续拆：[前向早停](early-stop.md) · [反向重走列表](backward.md)。

[本篇星系](../gaussian-splatting.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/gaussian-splatting-2308.04079/README.md) · [原文依据](https://arxiv.org/abs/2308.04079v1)
