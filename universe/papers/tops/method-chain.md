# 本篇方法链路 · TOPS

先用标准flow matching暖启动，把专家动作块沿逆流拉回噪声空间，按训练任务建立bank，再以低秩协方差高斯混合MPPCA拟合任务源。根据源/动作协方差的高斯最优输运方向识别需要扩张的轴，只在这些方向采用先慢后快插值，其他方向保留线性。固定源和schedule继续训练同一速度网络；语言selector选已知任务源。推理的一步采用依序两次网络求值的schedule-aware两半步方法，即NFE=2，不是一次前向。

先用标准flow matching暖启动，把专家动作块沿逆流拉回噪声空间，按训练任务建立bank，再以低秩协方差高斯混合MPPCA拟合任务源。根据源/动作协方差的高斯最优输运方向识别需要扩张的轴，只在这些方向采用先慢后快插值，其他方向保留线性。固定源和schedule继续训练同一速度网络；语言selector选已知任务源。推理的一步采用依序两次网络求值的schedule-aware两半步方法，即NFE=2，不是一次前向。

[本篇星系](../tops.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/tops.md) · [原文依据](https://arxiv.org/abs/2610.36694v1)
