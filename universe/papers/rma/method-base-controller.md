# 状态、旧动作与条件共同决定新动作 · RMA

基础策略拼接30维当前状态、12维上次动作和8维环境条件，输出12维目标关节角。

状态负责当前身体姿态，历史动作提供上一拍命令，潜变量提供环境条件；合计50维输入由一个隐藏宽度128的三层MLP处理。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md#31-基础策略特权信息怎样教出一套步态)

继续拆：[目标角经PD变成关节力矩](method-joint-pd.md) · [没有视觉的30维状态](method-proprioception.md)。

[本篇星系](../rma.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md) · [原文依据](https://www.roboticsproceedings.org/rss17/p011.pdf)
