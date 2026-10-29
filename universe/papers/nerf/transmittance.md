# 累积透射 · NeRF

光线走到某个位置还未被前方遮挡的比例。

T是前段密度积分的负指数，远处贡献受前方遮挡影响。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/nerf-2003.08934/README.md#4-体渲染沿途收颜色还得看前面挡了多少)

继续拆：[前向alpha合成](alpha-composite.md)。

[本篇星系](../nerf.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/nerf-2003.08934/README.md) · [原文依据](https://arxiv.org/abs/2003.08934v2)
