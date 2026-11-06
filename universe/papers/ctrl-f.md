# Ctrl-F 星系

Ctrl-F: Force as an Interface for Humanoid Loco-Manipulation

**导读** · Locomotion 与运动适应

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/ctrl-f.md) · [原文](https://arxiv.org/abs/2611.05507v1) · [评分卡](../../leaderboard/papers/ctrl-f/README.md)

低层运动–力跟踪器读取参考动作、本体状态与每接触刚体三维力，输出全身关节位置目标。无物体训练时按可施力mask采样f并施加−f，沿原运动跟踪目标学习；力幅度从零递增。冻结低层后，高层读取机器人/物体参考、物体接触点、物体实测状态和本体状态输出f。解析教师用PD位姿速度反馈、Newton–Euler及重力/摩擦补偿求六维W*，再按Gf≈W*和可行力集合分配。教师使用训练时真实质量；高层用在策略访问状态上的模仿目标和PPO联合训练，模仿权重衰减。部署不输入质量或测得接触力，仍依赖AprilTag物体姿态。

## 技术挂点

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

- [全身控制与执行](../concepts/wbc.md)：将运动目标、机器人状态和约束转成关节目标或力矩，协调腿、手臂与底盘。

- [示范模仿](../concepts/imitation.md)：从专家、人类或教师策略的行为学习动作，研究数据、表示和执行误差。

- [动作先验](../concepts/motion-prior.md)：从运动数据学习自然动作规律，再把它接进物理控制或技能选择。

- [分层技能与计划](../concepts/skills.md)：高层选择目标或技能，低层负责具体执行，层次之间有明确接口。

- [强化学习](../concepts/rl.md)：通过奖励和值评估改进策略，研究动作如何改变长期回报。

- [PPO 与并行模拟](../concepts/ppo.md)：用受约束的策略更新与大量模拟轨迹训练控制；并行度改变每轮数据和训练开销。

- [行为克隆](../concepts/bc.md)：直接监督观测到动作的映射，不必在每次更新中根据奖励搜索。

- [特权训练信息](../concepts/privileged.md)：训练用额外环境真值或教师信息，部署另用可获取输入估计或模仿。

- [环境适应](../concepts/adaptation.md)：根据历史观测或环境信息调整策略，使动力学或地形变化仍可处理。

- [仿真到实机](../concepts/sim2real.md)：处理仿真动力学、感知和真实系统间的差异，通过随机化、辨识、残差或适配来迁移。

- [机器人数据与评测](../concepts/data.md)：统一观测、动作、任务与评测条件，判断数据多样性如何影响泛化。

## 本篇行星与卫星

- [动作表示](ctrl-f/action.md) · 初读挂点
- [全身控制与执行](ctrl-f/wbc.md) · 初读挂点
- [示范模仿](ctrl-f/imitation.md) · 初读挂点
- [动作先验](ctrl-f/motion-prior.md) · 初读挂点
- [分层技能与计划](ctrl-f/skills.md) · 初读挂点
- [强化学习](ctrl-f/rl.md) · 初读挂点
- [PPO 与并行模拟](ctrl-f/ppo.md) · 初读挂点
- [行为克隆](ctrl-f/bc.md) · 初读挂点
- [特权训练信息](ctrl-f/privileged.md) · 初读挂点
- [环境适应](ctrl-f/adaptation.md) · 初读挂点
- [仿真到实机](ctrl-f/sim2real.md) · 初读挂点
- [机器人数据与评测](ctrl-f/data.md) · 初读挂点
- [本篇方法链路](ctrl-f/method-chain.md) · 初读挂点
- [动作像，不等于接触力够](ctrl-f/cf-problem.md) · 初读挂点
- [几何接触、抗扰与主动施力](ctrl-f/cf-related.md) · 初读挂点
- [一层跟动作，一层发力指令](ctrl-f/cf-hierarchy.md) · 初读挂点
- [没有物体，怎样学会施力](ctrl-f/cf-inverse.md) · 初读挂点
- [负载掩码限定能施力的身体](ctrl-f/cf-mask.md) · 初读挂点
- [先跟稳，再逐步增加指令力](ctrl-f/cf-curriculum.md) · 初读挂点
- [从物体误差决定该多用多少力](ctrl-f/cf-force-planner.md) · 初读挂点
- [用物体动力学构造教师力](ctrl-f/cf-analytical.md) · 初读挂点
- [抓取矩阵连接接触力和物体力矩](ctrl-f/cf-allocation.md) · 初读挂点
- [在自己走到的状态学教师，再用奖励修正](ctrl-f/cf-annealed.md) · 初读挂点
- [九种任务对应三套策略对](ctrl-f/cf-families.md) · 初读挂点
- [把物体质量和接触摩擦一起看](ctrl-f/cf-objects.md) · 初读挂点
- [姿态误差、存活和物体成功分开读](ctrl-f/cf-metrics.md) · 初读挂点
- [零力条件下仍可跟踪动作](ctrl-f/cf-zero-load.md) · 初读挂点
- [只改指令，外力轨迹保持一致](ctrl-f/cf-command-test.md) · 初读挂点
- [增加质量暴露力盲跟踪的边界](ctrl-f/cf-mass-sweep.md) · 初读挂点
- [负载增加后，指令力按什么方向改变](ctrl-f/cf-adapt-gain.md) · 初读挂点
- [在线适应不依赖训练回合中必有质量突变](ctrl-f/cf-fixed-mass.md) · 初读挂点
- [模仿力指令，可能仍没把力传给物体](ctrl-f/cf-bc-rl.md) · 初读挂点
- [去掉教师的证据是定性观察](ctrl-f/cf-rl-only.md) · 初读挂点
- [命令30 N，秤读24.5 N](ctrl-f/cf-real-force.md) · 初读挂点
- [20 kg说的是推和踢的附加配重](ctrl-f/cf-real-load.md) · 初读挂点
- [抬箱九次成功的分母在哪里](ctrl-f/cf-real-raise.md) · 初读挂点
- [冻结指令能单独测上层的作用](ctrl-f/cf-real-adapt.md) · 初读挂点
- [力接口可用，动作与感知范围仍有限](ctrl-f/cf-limits.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
