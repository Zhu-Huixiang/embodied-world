# Walk in the Park 星系

Demonstrating A Walk in the Park: Learning to Walk in 20 Minutes With Model-Free Reinforcement Learning

**导读** · Locomotion 与运动适应

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/walk-in-the-park.md) · [原文](https://www.roboticsproceedings.org/rss19/p056.html) · [评分卡](../../leaderboard/papers/walk-in-the-park/README.md)

基于 SAC/DroQ 的 actor-critic 从实机回放数据学习，用较高更新比、Dropout 和归一化稳定值函数。策略直接输出关节目标，本体传感器提供状态和奖励，异步采样训练与仔细的动作空间设计减少等待。论文在室内外多种地面验证从头学走路，并在模拟中分析设计选择。

## 技术挂点

- [策略与价值学习](../concepts/actor-critic.md)：actor 产生动作，critic 估计长期收益；价值估计为策略改进提供方向。

- [闭环滚动与历史偏移](../concepts/rollout.md)：重复预测、执行或生成，把新观测或模型历史接回后续计算。

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

## 本篇行星与卫星

- [策略与价值学习](walk-in-the-park/actor-critic.md) · 初读挂点
- [闭环滚动与历史偏移](walk-in-the-park/rollout.md) · 初读挂点
- [动作表示](walk-in-the-park/action.md) · 初读挂点
- [本篇方法链路](walk-in-the-park/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
