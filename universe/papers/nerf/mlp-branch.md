# 密度颜色分支 · NeRF

八层位置MLP产生密度和特征，再接方向生成RGB。

60维位置编码→8×256；特征256+方向24→128→3。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/nerf-2003.08934/README.md#32-mlp-里面到底走了几步)

继续拆：[输入跳接](skip-input.md)。

[本篇星系](../nerf.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/nerf-2003.08934/README.md) · [原文依据](https://arxiv.org/abs/2003.08934v2)
