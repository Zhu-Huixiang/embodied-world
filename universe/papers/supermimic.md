# SuperMimic 星系

SuperMimic: Scaling Humanoid Whole-Body Control with One Differentiable World Model

**导读** · 动作先验与全身技能

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/supermimic.md) · [原文](https://arxiv.org/abs/2610.28480) · [评分卡](../../leaderboard/papers/supermimic/README.md)

先让当前策略在 MuJoCo Warp 中收集状态、动作与下一状态，存进回放池；一个共享可微动力学模型用8步自回归窗口拟合这些转移。策略更新时暂时固定模型参数，在模型里展开32步想象轨迹，把跟踪奖励经动作和状态的雅可比反传给策略，末端价值函数补上短视野外的回报。模拟器采样、世界模型拟合与策略改进交替进行，最终将跟踪策略部署到 Unitree G1。世界模型服务训练，不替换实机执行反馈。

## 技术挂点

- [世界模型](../concepts/world.md)：学习状态随动作或时间如何变化，用于预测、计划或训练策略。

- [动作条件动力学](../concepts/dynamics.md)：以当前状态和动作预测下一状态或分布，建立“做这个动作会发生什么”的计算接口。

- [想象轨迹训练](../concepts/imagination.md)：在学到的动力学里滚动状态，用预测奖励和值训练策略，从而增加决策训练数据。

- [策略与价值学习](../concepts/actor-critic.md)：actor 产生动作，critic 估计长期收益；价值估计为策略改进提供方向。

- [全身控制与执行](../concepts/wbc.md)：将运动目标、机器人状态和约束转成关节目标或力矩，协调腿、手臂与底盘。

- [仿真到实机](../concepts/sim2real.md)：处理仿真动力学、感知和真实系统间的差异，通过随机化、辨识、残差或适配来迁移。

- [运动重定向](../concepts/retarget.md)：把人或另一种机器人的运动转换到目标本体的关节、末端与可达范围。

## 本篇行星与卫星

- [世界模型](supermimic/world.md) · 初读挂点
- [动作条件动力学](supermimic/dynamics.md) · 初读挂点
- [想象轨迹训练](supermimic/imagination.md) · 初读挂点
- [策略与价值学习](supermimic/actor-critic.md) · 初读挂点
- [全身控制与执行](supermimic/wbc.md) · 初读挂点
- [仿真到实机](supermimic/sim2real.md) · 初读挂点
- [运动重定向](supermimic/retarget.md) · 初读挂点
- [本篇方法链路](supermimic/method-chain.md) · 初读挂点
- [模拟器—模型—策略交替训练](supermimic/loop.md) · 初读挂点
- [回放池与8步模型拟合](supermimic/replay.md) · 初读挂点
- [随机化环境上下文](supermimic/context.md) · 初读挂点
- [32步想象与时间反传](supermimic/bptt.md) · 初读挂点
- [末端价值与短段想象](supermimic/critic.md) · 初读挂点
- [动作条件的全身跟踪](supermimic/motion.md) · 初读挂点
- [训练动作库覆盖评测](supermimic/coverage.md) · 初读挂点
- [GPU小时与比较条件](supermimic/compute.md) · 初读挂点
- [G1实机迁移](supermimic/transfer.md) · 初读挂点
- [速度命令接口](supermimic/velocity.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
