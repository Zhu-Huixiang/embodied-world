# 不同基线回答不同适应问题 · RMA

Robust去掉环境条件，SysID预测物理参数，AWR用测试环境采样优化潜变量，Expert直接拿真值条件。

无适应消融与Robust不是同一个比较；Expert是仿真可用的参照，不是现实中白得的控制器。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md#53-仿真把适应模块单独拿出来比)

继续拆：[在episode内部改条件的仿真测试](method-dynamic-test.md) · [成功率、站立时长与接触代价分开看](method-metric-tradeoffs.md)。

[本篇星系](../rma.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md) · [原文依据](https://www.roboticsproceedings.org/rss17/p011.pdf)
