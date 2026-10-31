# RMA 星系

RMA: Rapid Motor Adaptation for Legged Robots

**已精讲** · Locomotion 与运动适应

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md) · [原文](https://www.roboticsproceedings.org/rss17/p011.html) · [评分卡](../../leaderboard/papers/rma/README.md)

训练利用特权环境信息的基础策略，部署用状态动作历史估计环境编码，在线适配腿足控制。

## 技术挂点

- [强化学习](../concepts/rl.md)：通过奖励和值评估改进策略，研究动作如何改变长期回报。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md#31-基础策略特权信息怎样教出一套步态)

- [PPO 与并行模拟](../concepts/ppo.md)：用受约束的策略更新与大量模拟轨迹训练控制；并行度改变每轮数据和训练开销。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md#42-网络与训练预算)

- [特权训练信息](../concepts/privileged.md)：训练用额外环境真值或教师信息，部署另用可获取输入估计或模仿。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md#31-基础策略特权信息怎样教出一套步态)

- [环境适应](../concepts/adaptation.md)：根据历史观测或环境信息调整策略，使动力学或地形变化仍可处理。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md#32-适应模块从半秒经历估计控制条件)

- [仿真到实机](../concepts/sim2real.md)：处理仿真动力学、感知和真实系统间的差异，通过随机化、辨识、残差或适配来迁移。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md#41-环境与动作接口)

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md#41-环境与动作接口)

- [闭环滚动与历史偏移](../concepts/rollout.md)：重复预测、执行或生成，把新观测或模型历史接回后续计算。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md#32-适应模块从半秒经历估计控制条件)

## 本篇行星与卫星

- [强化学习](rma/rl.md) · 已讲解
- [PPO 与并行模拟](rma/ppo.md) · 已讲解
- [特权训练信息](rma/privileged.md) · 已讲解
- [环境适应](rma/adaptation.md) · 已讲解
- [仿真到实机](rma/sim2real.md) · 已讲解
- [动作表示](rma/action.md) · 已讲解
- [闭环滚动与历史偏移](rma/rollout.md) · 已讲解
- [本篇方法链路](rma/method-chain.md) · 已讲解
- [走动中的动力学变化](rma/method-adaptation-problem.md) · 已讲解
- [为控制学习的八维条件](rma/method-control-latent.md) · 已讲解
- [不必唯一辨认物理参数](rma/method-identifiability.md) · 已讲解
- [仿真中的17维环境因素](rma/method-privileged-vector.md) · 已讲解
- [局部地高压成一个标量](rma/method-local-height.md) · 已讲解
- [状态、旧动作与条件共同决定新动作](rma/method-base-controller.md) · 已讲解
- [目标角经PD变成关节力矩](rma/method-joint-pd.md) · 已讲解
- [没有视觉的30维状态](rma/method-proprioception.md) · 已讲解
- [先共同训练策略与环境编码器](rma/method-joint-ppo.md) · 已讲解
- [向前走之外还要付运动代价](rma/method-natural-reward.md) · 已讲解
- [做功与动作平滑是不同约束](rma/method-work-smoothness.md) · 已讲解
- [先学会动，再加强代价](rma/method-penalty-curriculum.md) · 已讲解
- [半秒历史估计当前控制条件](rma/method-history-adapter.md) · 已讲解
- [用仿真真值编码监督适应器](rma/method-latent-supervision.md) · 已讲解
- [让训练历史包含自己的失误](rma/method-on-policy-history.md) · 已讲解
- [时间卷积提取动作响应模式](rma/method-temporal-cnn.md) · 已讲解
- [100Hz动作与10Hz估计分开运行](rma/method-asynchronous-loops.md) · 已讲解
- [在线变化的是条件，不是权重](rma/method-frozen-deployment.md) · 已讲解
- [在变化的仿真动力学中练走路](rma/method-randomized-simulator.md) · 已讲解
- [地形变化帮助学习抬脚与稳步](rma/method-fractal-terrain.md) · 已讲解
- [部署省适应数据不等于训练便宜](rma/method-training-budget.md) · 已讲解
- [不同基线回答不同适应问题](rma/method-comparator-design.md) · 已讲解
- [在episode内部改条件的仿真测试](rma/method-dynamic-test.md) · 已讲解
- [成功率、站立时长与接触代价分开看](rma/method-metric-tradeoffs.md) · 已讲解
- [实机台阶结果的条件与样本](rma/method-real-step-tests.md) · 已讲解
- [打滑后潜变量与步态一起改变](rma/method-slip-response.md) · 已讲解
- [突然负载带来的另一种适应](rma/method-payload-response.md) · 已讲解
- [接触历史无法提前看到障碍](rma/method-blind-limit.md) · 已讲解
- [未见地形上的迁移范围](rma/method-outdoor-scope.md) · 已讲解

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
