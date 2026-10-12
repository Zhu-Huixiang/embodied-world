# 本篇方法链路 · Deep WBC

同一个网络接收底盘、腿、手臂状态和任务命令，输出六维手臂与十二维腿部关节目标，再由 PD 转为力矩。Advantage Mixing 把移动和操作的收益联系起来，Regularized Online Adaptation 对齐历史估计与训练环境信息。实验比较分开的控制器、未协调策略和适应方法，并在四足机械臂上验证。

同一个网络接收底盘、腿、手臂状态和任务命令，输出六维手臂与十二维腿部关节目标，再由 PD 转为力矩。Advantage Mixing 把移动和操作的收益联系起来，Regularized Online Adaptation 对齐历史估计与训练环境信息。实验比较分开的控制器、未协调策略和适应方法，并在四足机械臂上验证。

[本篇星系](../deep-whole-body-control.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/deep-whole-body-control.md) · [原文依据](https://proceedings.mlr.press/v205/fu23a.html)
