# 像素监督与可微渲染 · NeRF

用粗细预测RGB与观测像素的平方误差训练。

梯度经过合成更新密度颜色，粗网也需监督以可靠分配采样。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/nerf-2003.08934/README.md#53-训练照片给像素答案不给每个点的标准密度)

[本篇星系](../nerf.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/nerf-2003.08934/README.md) · [原文依据](https://arxiv.org/abs/2003.08934v2)
