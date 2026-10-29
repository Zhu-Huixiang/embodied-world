# 采样硬件与批量账单 · DDPM

训练一步抽题，生成一批执行完整链。

TPUv3-8上256张CIFAR约17秒、128张256²约300秒，不能跨批量写成单图延迟。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md#42-消融光把输出改成噪声还不够)

[本篇星系](../ddpm.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md) · [原文依据](https://arxiv.org/pdf/2006.11239v2)
