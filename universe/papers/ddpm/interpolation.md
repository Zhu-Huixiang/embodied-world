# 带噪状态插值 · DDPM

两源图加噪到同t后混合并反向生成。

λ控制混合比例；先扩散再混合比直接像素叠图能重组结构，不许诺每个语义属性独立控制。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md#44-插值直接叠两张脸为什么容易叠出双影)

[本篇星系](../ddpm.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md) · [原文依据](https://arxiv.org/pdf/2006.11239v2)
