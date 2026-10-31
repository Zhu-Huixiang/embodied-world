# 半秒历史估计当前控制条件 · RMA

适应模块使用最近50步状态与动作预测8维潜变量，在100Hz控制下对应约0.5秒历史。

历史中动作指令与身体实际响应的配对包含环境线索。适应并不是重新识别一套精确物理模型后再规划。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md#32-适应模块从半秒经历估计控制条件)

继续拆：[用仿真真值编码监督适应器](method-latent-supervision.md) · [时间卷积提取动作响应模式](method-temporal-cnn.md)。

[本篇星系](../rma.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md) · [原文依据](https://www.roboticsproceedings.org/rss17/p011.pdf)
