# 在episode内部改条件的仿真测试 · RMA

测试按每步0.01概率重新采样环境参数，让适应速度进入比较。

TableII按3次随机初始化、每次1000个episode平均：RMA成功率73.5%，Robust62.4%，无适应52.1%，Expert76.2%。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md#53-仿真把适应模块单独拿出来比)

[本篇星系](../rma.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md) · [原文依据](https://www.roboticsproceedings.org/rss17/p011.pdf)
