# 100Hz动作与10Hz估计分开运行 · RMA

基础策略每秒产生100次目标角，适应器每秒约更新10次环境条件，二者异步。

每次动作使用最新可用的潜变量，不等待一次新估计。这样把相对慢的环境条件变化与较快的机器人状态变化分开。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md#33-异步部署腿快一点判断慢一点)

继续拆：[在线变化的是条件，不是权重](method-frozen-deployment.md)。

[本篇星系](../rma.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md) · [原文依据](https://www.roboticsproceedings.org/rss17/p011.pdf)
