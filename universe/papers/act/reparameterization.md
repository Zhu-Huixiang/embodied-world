# 重参数采样 · ACT / ALOHA

z=mu+s乘epsilon，把随机噪声与可学习参数分开。

epsilon标准高斯；梯度经mu和s回传，s是标准差。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/act-2304.13705/README.md#43-cvae同一幅画面可以有不同的后续走法)

[本篇星系](../act.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/act-2304.13705/README.md) · [原文依据](https://www.roboticsproceedings.org/rss19/p016.html)
