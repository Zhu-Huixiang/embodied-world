# Cal-QL 星系

Cal-QL: Calibrated Offline RL Pre-Training for Efficient Online Fine-Tuning

**导读** · 强化学习与离线决策

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/cal-ql.md) · [原文](https://proceedings.neurips.cc/paper_files/paper/2023/hash/c44a04289beaf0a7d968a94066a1d696-Abstract-Conference.html) · [评分卡](../../leaderboard/papers/cal-ql/README.md)

Cal-QL 保留 CQL 的保守价值学习，同时把学习策略的价值锚定在一个可估计参考策略的价值之上。这样在线新数据进入时，低估的旧 Q 不至于诱导策略先丢掉离线技能。原文分别分析初期遗忘、价值尺度变化，并在导航、操作和图像输入微调任务上比较。

## 技术挂点

- [离线强化学习](../concepts/offline.md)：从已有轨迹学习决策，训练时不能自由去环境补齐数据外动作的后果。

- [价值估计与校准](../concepts/value.md)：估计未来累积收益，再用保守、分位或参考价值等约束减少误导。

- [策略与价值学习](../concepts/actor-critic.md)：actor 产生动作，critic 估计长期收益；价值估计为策略改进提供方向。

## 本篇行星与卫星

- [离线强化学习](cal-ql/offline.md) · 初读挂点
- [价值估计与校准](cal-ql/value.md) · 初读挂点
- [策略与价值学习](cal-ql/actor-critic.md) · 初读挂点
- [本篇方法链路](cal-ql/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
