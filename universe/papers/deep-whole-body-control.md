# Deep WBC 星系

Deep Whole-Body Control: Learning a Unified Policy for Manipulation and Locomotion

**导读** · Locomotion 与运动适应

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/deep-whole-body-control.md) · [原文](https://proceedings.mlr.press/v205/fu23a.html) · [评分卡](../../leaderboard/papers/deep-whole-body-control/README.md)

同一个网络接收底盘、腿、手臂状态和任务命令，输出六维手臂与十二维腿部关节目标，再由 PD 转为力矩。Advantage Mixing 把移动和操作的收益联系起来，Regularized Online Adaptation 对齐历史估计与训练环境信息。实验比较分开的控制器、未协调策略和适应方法，并在四足机械臂上验证。

## 技术挂点

- [全身控制与执行](../concepts/wbc.md)：将运动目标、机器人状态和约束转成关节目标或力矩，协调腿、手臂与底盘。

- [环境适应](../concepts/adaptation.md)：根据历史观测或环境信息调整策略，使动力学或地形变化仍可处理。

- [强化学习](../concepts/rl.md)：通过奖励和值评估改进策略，研究动作如何改变长期回报。

## 本篇行星与卫星

- [全身控制与执行](deep-whole-body-control/wbc.md) · 初读挂点
- [环境适应](deep-whole-body-control/adaptation.md) · 初读挂点
- [强化学习](deep-whole-body-control/rl.md) · 初读挂点
- [本篇方法链路](deep-whole-body-control/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
