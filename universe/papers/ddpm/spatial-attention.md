# 16×16空间注意力 · DDPM

256个位置产生Q/K/V并互相汇总。

教学单头Q/K/V为256×d，匹配矩阵256×256；d不冒充原文给定超参。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md#36-打开-b-区u-net-里面怎样处理图像和时间)

[本篇星系](../ddpm.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md) · [原文依据](https://arxiv.org/pdf/2006.11239v2)
