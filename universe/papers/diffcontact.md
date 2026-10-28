# DiffContact 星系

Differentiable Contact Dynamics for Legged Locomotion: Policy Learning and Contact-Implicit Trajectory Optimization

**导读** · Locomotion 与运动适应

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/diffcontact.md) · [原文](https://arxiv.org/abs/2610.35852v1) · [评分卡](../../leaderboard/papers/diffcontact/README.md)

前向继续用硬接触模拟器生成轨迹，只在反向替换接触冲量的敏感度。方法对含de Saxcé修正的库仑摩擦二阶锥互补条件做完整锥中心路径松弛，从硬接触解出发用Newton迭代找到反向求导的评估点，组装状态/动作转移Jacobian，再供BPTT更新策略或DDP/iLQR优化轨迹。法向与切向一起松弛，梯度才有机会指向离地、粘住和滑动这些邻近模式；松弛参数趋零时回到固定接触模式的精确敏感度。

## 技术挂点

- [动作条件动力学](../concepts/dynamics.md)：以当前状态和动作预测下一状态或分布，建立“做这个动作会发生什么”的计算接口。

- [强化学习](../concepts/rl.md)：通过奖励和值评估改进策略，研究动作如何改变长期回报。

- [闭环滚动与历史偏移](../concepts/rollout.md)：重复预测、执行或生成，把新观测或模型历史接回后续计算。

- [PPO 与并行模拟](../concepts/ppo.md)：用受约束的策略更新与大量模拟轨迹训练控制；并行度改变每轮数据和训练开销。

- [仿真到实机](../concepts/sim2real.md)：处理仿真动力学、感知和真实系统间的差异，通过随机化、辨识、残差或适配来迁移。

## 本篇行星与卫星

- [动作条件动力学](diffcontact/dynamics.md) · 初读挂点
- [强化学习](diffcontact/rl.md) · 初读挂点
- [闭环滚动与历史偏移](diffcontact/rollout.md) · 初读挂点
- [PPO 与并行模拟](diffcontact/ppo.md) · 初读挂点
- [仿真到实机](diffcontact/sim2real.md) · 初读挂点
- [本篇方法链路](diffcontact/method-chain.md) · 初读挂点
- [分离、粘着与滑动](diffcontact/modes.md) · 初读挂点
- [保留硬接触前向](diffcontact/hard.md) · 初读挂点
- [完整摩擦锥中心路径](diffcontact/cone.md) · 初读挂点
- [从硬接触解求反向评估点](diffcontact/newton.md) · 初读挂点
- [冲量敏感度与转移Jacobian](diffcontact/jacobian.md) · 初读挂点
- [20步短段策略反传](diffcontact/bptt.md) · 初读挂点
- [同前向三种梯度对照](diffcontact/ablate.md) · 初读挂点
- [短时训练后上四足实机](diffcontact/hardware.md) · 初读挂点
- [PPO样本和时间对照](diffcontact/method-ppo.md) · 初读挂点
- [Newton残差与锥可行性](diffcontact/feasible.md) · 初读挂点
- [接触隐式轨迹优化](diffcontact/cito.md) · 初读挂点
- [点足与接触几何的边界](diffcontact/geometry.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
