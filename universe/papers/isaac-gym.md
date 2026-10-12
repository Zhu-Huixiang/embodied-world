# Isaac Gym 星系

Isaac Gym: High Performance GPU Based Physics Simulation For Robot Learning

**导读** · 强化学习与离线决策

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/isaac-gym.md) · [原文](https://datasets-benchmarks-proceedings.neurips.cc/paper/2021/hash/28dd2c7955ce926456240b2ff0100bde-Abstract-round2.html) · [评分卡](../../leaderboard/papers/isaac-gym/README.md)

GPU PhysX 缓冲包装为 PyTorch tensor；观测、奖励、动作、并行 rollout 与 PPO 保持 GPU，省去 CPU↔GPU 往返。

## 技术挂点

- [PPO 与并行模拟](../concepts/ppo.md)：用受约束的策略更新与大量模拟轨迹训练控制；并行度改变每轮数据和训练开销。

- [强化学习](../concepts/rl.md)：通过奖励和值评估改进策略，研究动作如何改变长期回报。

## 本篇行星与卫星

- [PPO 与并行模拟](isaac-gym/ppo.md) · 初读挂点
- [强化学习](isaac-gym/rl.md) · 初读挂点
- [本篇方法链路](isaac-gym/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
