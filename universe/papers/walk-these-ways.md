# Walk These Ways 星系

Walk These Ways: Tuning Robot Control for Generalization with Multiplicity of Behavior

**导读** · Locomotion 与运动适应

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/walk-these-ways.md) · [原文](https://proceedings.mlr.press/v205/margolis23a.html) · [评分卡](../../leaderboard/papers/walk-these-ways/README.md)

一个策略同时接收三维速度命令和八维行为参数，后者控制足端相位、频率、身体姿态与抬脚等走法。历史本体观测与这些命令共同输入网络，输出十二个关节的位置目标。测试时人可以调整行为参数，在不重训情况下为新任务挑选合适步态。

## 技术挂点

- [分层技能与计划](../concepts/skills.md)：高层选择目标或技能，低层负责具体执行，层次之间有明确接口。

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

- [环境适应](../concepts/adaptation.md)：根据历史观测或环境信息调整策略，使动力学或地形变化仍可处理。

## 本篇行星与卫星

- [分层技能与计划](walk-these-ways/skills.md) · 初读挂点
- [动作表示](walk-these-ways/action.md) · 初读挂点
- [环境适应](walk-these-ways/adaptation.md) · 初读挂点
- [本篇方法链路](walk-these-ways/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
