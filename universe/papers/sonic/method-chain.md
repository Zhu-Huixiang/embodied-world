# 本篇方法链路 · SONIC

机器人/人体/稀疏混合命令分别编码到 FSQ 共享运动 token；同一控制解码器结合10步本体历史输出29关节目标，由PD执行。PPO与运动重建、token对齐和cycle损失联合训练；上游实时运动规划或VLA预测64维token与14维手关节。

机器人/人体/稀疏混合命令分别编码到 FSQ 共享运动 token；同一控制解码器结合10步本体历史输出29关节目标，由PD执行。PPO与运动重建、token对齐和cycle损失联合训练；上游实时运动规划或VLA预测64维token与14维手关节。

[本篇星系](../sonic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/sonic.md) · [原文依据](https://www.science.org/doi/10.1126/scirobotics.aed4592)
