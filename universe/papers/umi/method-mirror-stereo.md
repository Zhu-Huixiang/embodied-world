# 侧镜在单张图内提供隐式立体 · UMI

两块镜面等价于不同光心的虚拟相机，为接触和遮挡提供额外视角。

策略使用RGB中的镜区线索，没有新增显式深度图或双目深度监督模块。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md#32-hd2与hd3鱼眼看周边镜子补视差)

继续拆：[翻转镜区并交换左右](method-mirror-swap.md)。

[本篇星系](../umi.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md) · [原文依据](https://www.roboticsproceedings.org/rss20/p045.pdf)
