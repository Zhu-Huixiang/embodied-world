# 粗细网络采样 · NeRF

粗网络合成权重指导细网络查询位置。

粗64点，新细128点，细网在192点上评估；总256次查询。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/nerf-2003.08934/README.md#52-分层采样先打草稿再把算力花到画面上)

继续拆：[逆CDF采样](inverse-cdf.md)。

[本篇星系](../nerf.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/nerf-2003.08934/README.md) · [原文依据](https://arxiv.org/abs/2003.08934v2)
