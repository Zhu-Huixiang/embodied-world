# 在线变化的是条件，不是权重 · RMA

实机上适应器持续前向推断，网络参数保持训练完成后的固定值。

论文部署算法只有历史读取、潜变量预测和动作计算，没有在线梯度优化；“在线适应”不能解释为边走边训练神经网络。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md#33-异步部署腿快一点判断慢一点)

[本篇星系](../rma.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md) · [原文依据](https://www.roboticsproceedings.org/rss17/p011.pdf)
