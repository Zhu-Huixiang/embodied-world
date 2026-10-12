# SONIC 星系

SONIC: Supersizing Motion Tracking for Natural Humanoid Whole-Body Control

**导读** · Locomotion 与运动适应

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/sonic.md) · [原文](https://www.science.org/doi/10.1126/scirobotics.aed4592) · [评分卡](../../leaderboard/papers/sonic/README.md)

机器人/人体/稀疏混合命令分别编码到 FSQ 共享运动 token；同一控制解码器结合10步本体历史输出29关节目标，由PD执行。PPO与运动重建、token对齐和cycle损失联合训练；上游实时运动规划或VLA预测64维token与14维手关节。

## 技术挂点

- [离散编码与量化](../concepts/quantization.md)：把连续向量或信号映射到有限码。动作、视频潜变量与世界模型状态都可能采用这种表示，码本和训练目标各不相同。

- [全身控制与执行](../concepts/wbc.md)：将运动目标、机器人状态和约束转成关节目标或力矩，协调腿、手臂与底盘。

- [PPO 与并行模拟](../concepts/ppo.md)：用受约束的策略更新与大量模拟轨迹训练控制；并行度改变每轮数据和训练开销。

## 本篇行星与卫星

- [离散编码与量化](sonic/quantization.md) · 初读挂点
- [全身控制与执行](sonic/wbc.md) · 初读挂点
- [PPO 与并行模拟](sonic/ppo.md) · 初读挂点
- [本篇方法链路](sonic/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
