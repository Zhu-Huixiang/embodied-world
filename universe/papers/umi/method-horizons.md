# 动作horizon与去噪步数不同 · UMI

Table A1列动作执行 horizon T_a=6；训练噪声时间步数50，推理采用16步DDIM去噪。

6表示每轮执行窗口，不能据此补造完整动作预测窗口；50与16属于生成器内部噪声时间，不是机器人控制时刻。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md#45-接上diffusion-policy观察怎样变成一段动作)

[本篇星系](../umi.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md) · [原文依据](https://umi-gripper.github.io/umi.pdf)
