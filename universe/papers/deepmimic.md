# DeepMimic 星系

DeepMimic: Example-Guided Deep Reinforcement Learning of Physics-Based Character Skills

**已精讲** · 动作先验与全身技能

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md) · [原文](https://xbpeng.github.io/projects/DeepMimic/) · [评分卡](../../leaderboard/papers/deepmimic/README.md)

任务奖励与参考动作跟踪奖励共同训练物理角色策略，使动作技能能在动态扰动后恢复。

## 技术挂点

- [动作先验](../concepts/motion-prior.md)：从运动数据学习自然动作规律，再把它接进物理控制或技能选择。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md#53-奖励)

- [强化学习](../concepts/rl.md)：通过奖励和值评估改进策略，研究动作如何改变长期回报。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md#4-背景奖励怎样改掉下一次动作)

- [全身控制与执行](../concepts/wbc.md)：将运动目标、机器人状态和约束转成关节目标或力矩，协调腿、手臂与底盘。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md#3-方法总览从参考姿态到物理动作)

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md#51-状态与动作)

- [示范模仿](../concepts/imitation.md)：从专家、人类或教师策略的行为学习动作，研究数据、表示和执行误差。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md#53-奖励)

- [策略与价值学习](../concepts/actor-critic.md)：actor 产生动作，critic 估计长期收益；价值估计为策略改进提供方向。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md#4-背景奖励怎样改掉下一次动作)

- [价值估计与校准](../concepts/value.md)：估计未来累积收益，再用保守、分位或参考价值等约束减少误导。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md#4-背景奖励怎样改掉下一次动作)

- [PPO 与并行模拟](../concepts/ppo.md)：用受约束的策略更新与大量模拟轨迹训练控制；并行度改变每轮数据和训练开销。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md#4-背景奖励怎样改掉下一次动作)

- [softmax 与温度](../concepts/softmax.md)：对候选分数取指数后归一化为总和为 1 的概率。温度控制分差如何影响概率。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md#7-多技能三种不同的组织方式)

- [分层技能与计划](../concepts/skills.md)：高层选择目标或技能，低层负责具体执行，层次之间有明确接口。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md#7-多技能三种不同的组织方式)

- [运动重定向](../concepts/retarget.md)：把人或另一种机器人的运动转换到目标本体的关节、末端与可达范围。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md#103-动作重定向)

## 本篇行星与卫星

- [动作先验](deepmimic/motion-prior.md) · 已讲解
- [强化学习](deepmimic/rl.md) · 已讲解
- [全身控制与执行](deepmimic/wbc.md) · 已讲解
- [动作表示](deepmimic/action.md) · 已讲解
- [示范模仿](deepmimic/imitation.md) · 已讲解
- [策略与价值学习](deepmimic/actor-critic.md) · 已讲解
- [价值估计与校准](deepmimic/value.md) · 已讲解
- [PPO 与并行模拟](deepmimic/ppo.md) · 已讲解
- [softmax 与温度](deepmimic/softmax.md) · 已讲解
- [分层技能与计划](deepmimic/skills.md) · 已讲解
- [运动重定向](deepmimic/retarget.md) · 已讲解
- [本篇方法链路](deepmimic/method-chain.md) · 已讲解
- [动作风格与任务目标](deepmimic/goal-and-style.md) · 已讲解
- [运动学参考与物理控制](deepmimic/kinematic-vs-physical.md) · 已讲解
- [目标朝向到力矩闭环](deepmimic/pd-control-loop.md) · 已讲解
- [参考数据的两条训练通道](deepmimic/reference-two-channels.md) · 已讲解
- [折扣回报与优势](deepmimic/discounted-return.md) · 已讲解
- [多步与λ回报](deepmimic/lambda-return.md) · 已讲解
- [GAE把回报变为相对优势](deepmimic/gae-advantage.md) · 已讲解
- [root局部身体特征](deepmimic/root-local-state.md) · 已讲解
- [相位时钟](deepmimic/phase-clock.md) · 已讲解
- [轴角与单轴目标动作](deepmimic/joint-target-action.md) · 已讲解
- [策略和物理的两级时钟](deepmimic/policy-physics-rates.md) · 已讲解
- [固定协方差高斯策略](deepmimic/gaussian-actor.md) · 已讲解
- [标量value网络](deepmimic/scalar-critic.md) · 已讲解
- [高度图特征支路](deepmimic/heightmap-cnn.md) · 已讲解
- [四项模仿奖励](deepmimic/imitation-four-terms.md) · 已讲解
- [四元数相对转角](deepmimic/quaternion-pose-error.md) · 已讲解
- [参考角速度的差分](deepmimic/finite-difference-velocity.md) · 已讲解
- [手脚世界位置误差](deepmimic/end-effector-world-error.md) · 已讲解
- [质心位置误差](deepmimic/center-of-mass-error.md) · 已讲解
- [模仿和任务的加权](deepmimic/task-imitation-mixture.md) · 已讲解
- [从交互batch到网络更新](deepmimic/rollout-update-loop.md) · 已讲解
- [PPO的有方向裁剪](deepmimic/ppo-clipped-surrogate.md) · 已讲解
- [统一超参及本体步长](deepmimic/training-hyperparameters.md) · 已讲解
- [参考状态初始化RSI](deepmimic/reference-state-initialization.md) · 已讲解
- [后半段价值反哺前半段](deepmimic/landing-before-takeoff.md) · 已讲解
- [失败接触提前终止ET](deepmimic/early-termination.md) · 已讲解
- [减少倒地无效样本](deepmimic/fallen-state-bias.md) · 已讲解
- [对多参考取max](deepmimic/max-reference-reward.md) · 已讲解
- [onehot显式点选技能](deepmimic/onehot-skill-selector.md) · 已讲解
- [价值引导的组合策略](deepmimic/value-composite-policy.md) · 已讲解
- [按周期选择与归一价值](deepmimic/cycle-level-selection.md) · 已讲解
- [四种仿真刚体角色](deepmimic/articulated-characters.md) · 已讲解
- [状态维数与自由度区分](deepmimic/axis-angle-dof.md) · 已讲解
- [方向速度的单侧奖励](deepmimic/heading-one-sided-reward.md) · 已讲解
- [命中目标的显式记忆](deepmimic/strike-memory-bit.md) · 已讲解
- [固定时点释放的投掷](deepmimic/fixed-release-throw.md) · 已讲解
- [先平地再复杂地形训练](deepmimic/terrain-progressive-training.md) · 已讲解
- [一维与二维地形范围](deepmimic/heightfield-scope.md) · 已讲解
- [归一回报不等于成功率](deepmimic/normalized-return-protocol.md) · 已讲解
- [短参考与大量交互并存](deepmimic/few-seconds-many-samples.md) · 已讲解
- [模仿与任务的删项实验](deepmimic/task-objective-ablation.md) · 已讲解
- [转向时更匹配转弯clip](deepmimic/walking-clip-switch.md) · 已讲解
- [Atlas复制参考后重训](deepmimic/atlas-retraining-boundary.md) · 已讲解
- [新环境和重力下重训](deepmimic/environment-physics-retraining.md) · 已讲解
- [消融另用固定起点评估](deepmimic/ablation-evaluation-shift.md) · 已讲解
- [接近回报隐藏不同动作](deepmimic/reward-behavior-mismatch.md) · 已讲解
- [单seed与三seed范围](deepmimic/seed-coverage.md) · 已讲解
- [固定相位的推力测试](deepmimic/phase-specific-push-test.md) · 已讲解
- [探索噪声的鲁棒性解释](deepmimic/noise-robustness-hypothesis.md) · 已讲解
- [时序、规模与成本局限](deepmimic/timing-library-cost-limits.md) · 已讲解

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
