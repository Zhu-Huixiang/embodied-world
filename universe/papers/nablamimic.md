# ∇Mimic 星系

∇Mimic: Ultra-Efficient Humanoid Control with Differentiable Simulation

**导读** · 动作先验与全身技能

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/nablamimic.md) · [原文](https://arxiv.org/abs/2610.41654v1) · [评分卡](../../leaderboard/papers/nablamimic/README.md)

在4096个64步窗口中沿MuJoCo接触动力学求导，逐反向时间步对每个样本的动作cotangent按批中位范数裁剪，再以固定弧度RMS步长构造目标动作、做8次小批回归。G1专用NablaEngine用每world一个warp及整控制步adjoint megakernel降低求导成本。保留TDλ critic、参考姿态残差和回放起点；训练导数在近自接触、近平行胶囊及饱和actuator处采用特定规则，并非处处无偏的精确梯度。

## 技术挂点

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

- [全身控制与执行](../concepts/wbc.md)：将运动目标、机器人状态和约束转成关节目标或力矩，协调腿、手臂与底盘。

- [动作条件动力学](../concepts/dynamics.md)：以当前状态和动作预测下一状态或分布，建立“做这个动作会发生什么”的计算接口。

- [强化学习](../concepts/rl.md)：通过奖励和值评估改进策略，研究动作如何改变长期回报。

- [策略与价值学习](../concepts/actor-critic.md)：actor 产生动作，critic 估计长期收益；价值估计为策略改进提供方向。

- [PPO 与并行模拟](../concepts/ppo.md)：用受约束的策略更新与大量模拟轨迹训练控制；并行度改变每轮数据和训练开销。

- [机器人数据与评测](../concepts/data.md)：统一观测、动作、任务与评测条件，判断数据多样性如何影响泛化。

## 本篇行星与卫星

- [动作表示](nablamimic/action.md) · 初读挂点
- [全身控制与执行](nablamimic/wbc.md) · 初读挂点
- [动作条件动力学](nablamimic/dynamics.md) · 初读挂点
- [强化学习](nablamimic/rl.md) · 初读挂点
- [策略与价值学习](nablamimic/actor-critic.md) · 初读挂点
- [PPO 与并行模拟](nablamimic/ppo.md) · 初读挂点
- [机器人数据与评测](nablamimic/data.md) · 初读挂点
- [本篇方法链路](nablamimic/method-chain.md) · 初读挂点
- [接触动力学为何让一阶策略学习爆炸](nablamimic/nm-problem.md) · 初读挂点
- [G1全身动作跟踪](nablamimic/nm-task.md) · 初读挂点
- [参考动作编码与本体历史解码](nablamimic/nm-actor.md) · 初读挂点
- [短窗回报与价值自举](nablamimic/nm-objective.md) · 初读挂点
- [同轨迹精确与模型梯度比较](nablamimic/nm-tail.md) · 初读挂点
- [反传内逐样本中位数裁剪](nablamimic/nm-clipping.md) · 初读挂点
- [定弧度动作目标](nablamimic/nm-target.md) · 初读挂点
- [一段求导窗口复用八次回归](nablamimic/nm-regress.md) · 初读挂点
- [动作目标界与实际策略更新](nablamimic/nm-bound.md) · 初读挂点
- [梯度链长度与critic依赖](nablamimic/nm-horizon.md) · 初读挂点
- [参考姿态加关节残差](nablamimic/nm-residual.md) · 初读挂点
- [回放起点与当前策略采样](nablamimic/nm-replay.md) · 初读挂点
- [终止屏蔽与训练跌倒惩罚](nablamimic/nm-fall.md) · 初读挂点
- [单机器人融合求导引擎](nablamimic/nm-engine.md) · 初读挂点
- [接触解最优条件的隐式求导](nablamimic/nm-adjoint.md) · 初读挂点
- [精确模式与训练导数规则](nablamimic/nm-guards.md) · 初读挂点
- [有限差分校验导数](nablamimic/nm-accuracy.md) · 初读挂点
- [一步物理连同梯度的计时](nablamimic/nm-speed.md) · 初读挂点
- [同算法更换仿真器](nablamimic/nm-isolation.md) · 初读挂点
- [整片段归一化回报评测](nablamimic/nm-eval.md) · 初读挂点
- [v1三seed训练效率](nablamimic/nm-results.md) · 初读挂点
- [官方报告、第三方复现与本地基线分层](nablamimic/nm-baselines.md) · 初读挂点
- [专用引擎与仿真适用范围](nablamimic/nm-limit.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
