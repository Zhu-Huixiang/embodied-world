# HALO 星系

Perceptive Humanoid Motion from Simulation

**导读** · 动作先验与全身技能

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/halo.md) · [原文](https://arxiv.org/abs/2611.06908v1) · [评分卡](../../leaderboard/papers/halo/README.md)

HALO先用INFINIGEN房间、KIMODO约束运动、场景摆放和第一视角渲染合成162698回合/296.3小时的视觉—指令—全身轨迹。冻结Qwen3.5-2B编码224×224RGB与文字，8层DiT以流匹配生成150×36的五秒骨盆相对计划；首15帧保持干净，学习接续135帧，并以15步Euler、约3Hz异步更新。低层先训练三类特权PPO专家，再按技能路由BC/DAgger蒸馏为深度学生，最后多critic PPO微调。共享跟踪器融合48×84深度、30步本体历史和计划，以50Hz输出29关节目标。上层VLM从自由语言选择有限技能并检查完成/重试，默认两台机载计算机协作。

## 技术挂点

- [Flow Matching](../concepts/flow.md)：给噪声到数据指定概率路径，回归沿路径的速度场；生成时数值积分这个场。

- [Diffusion Transformer](../concepts/dit.md)：用 Transformer 实现扩散模型的去噪网络，使 token 之间交换条件与目标信息。

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。

- [全身控制与执行](../concepts/wbc.md)：将运动目标、机器人状态和约束转成关节目标或力矩，协调腿、手臂与底盘。

- [PPO 与并行模拟](../concepts/ppo.md)：用受约束的策略更新与大量模拟轨迹训练控制；并行度改变每轮数据和训练开销。

- [教师学生蒸馏](../concepts/distill.md)：用教师的预测分布、特征或动作监督学生，把已有模型的可用信息迁移到学生。

- [特权训练信息](../concepts/privileged.md)：训练用额外环境真值或教师信息，部署另用可获取输入估计或模仿。

- [仿真到实机](../concepts/sim2real.md)：处理仿真动力学、感知和真实系统间的差异，通过随机化、辨识、残差或适配来迁移。

- [机器人数据与评测](../concepts/data.md)：统一观测、动作、任务与评测条件，判断数据多样性如何影响泛化。

- [动作先验](../concepts/motion-prior.md)：从运动数据学习自然动作规律，再把它接进物理控制或技能选择。

- [运动重定向](../concepts/retarget.md)：把人或另一种机器人的运动转换到目标本体的关节、末端与可达范围。

- [分层技能与计划](../concepts/skills.md)：高层选择目标或技能，低层负责具体执行，层次之间有明确接口。

## 本篇行星与卫星

- [Flow Matching](halo/flow.md) · 初读挂点
- [Diffusion Transformer](halo/dit.md) · 初读挂点
- [动作块](halo/chunk.md) · 初读挂点
- [全身控制与执行](halo/wbc.md) · 初读挂点
- [PPO 与并行模拟](halo/ppo.md) · 初读挂点
- [教师学生蒸馏](halo/distill.md) · 初读挂点
- [特权训练信息](halo/privileged.md) · 初读挂点
- [仿真到实机](halo/sim2real.md) · 初读挂点
- [机器人数据与评测](halo/data.md) · 初读挂点
- [动作先验](halo/motion-prior.md) · 初读挂点
- [运动重定向](halo/retarget.md) · 初读挂点
- [分层技能与计划](halo/skills.md) · 初读挂点
- [本篇方法链路](halo/method-chain.md) · 初读挂点
- [语义感知与物理接触是两层问题](halo/halo-problem.md) · 初读挂点
- [程序化房间怎样长出全身监督](halo/halo-data.md) · 初读挂点
- [省掉逐回合遥操作，仍要设计运动种子](halo/halo-seeds.md) · 初读挂点
- [先摆得下，再渲染看见什么](halo/halo-staging.md) · 初读挂点
- [296.3小时包含六个有限技能](halo/halo-corpus.md) · 初读挂点
- [保留下来的轨迹并非全过硬检查](halo/halo-filter.md) · 初读挂点
- [冻结语义编码器，学习运动解码器](halo/halo-generator.md) · 初读挂点
- [五秒运动写成150乘36](halo/halo-plan.md) · 初读挂点
- [从高斯噪声推向运动参考](halo/halo-flow.md) · 初读挂点
- [把已承诺的半秒作为干净前缀](halo/halo-prefix.md) · 初读挂点
- [50Hz跟踪器处理身体与接触](halo/halo-tracker.md) · 初读挂点
- [先按接触类型训练三类专家](halo/halo-experts.md) · 初读挂点
- [把正确专家路由给当前技能](halo/halo-distill.md) · 初读挂点
- [共享演员，分开评价不同技能](halo/halo-multicritic.md) · 初读挂点
- [机器人自己的遮挡也要进入深度](halo/halo-depth.md) · 初读挂点
- [跟上动作还要真的推动物体](halo/halo-contact.md) · 初读挂点
- [把自由请求分给有限技能](halo/halo-orchestrator.md) · 初读挂点
- [两台机载计算机分开语义与实时控制](halo/halo-onboard.md) · 初读挂点
- [把单技能与完整任务链分开统计](halo/halo-evaluation.md) · 初读挂点
- [实机91%是六技能平均](halo/halo-atomic-results.md) · 初读挂点
- [长链任务还会丢目标](halo/halo-chain-results.md) · 初读挂点
- [房间多样性支持陌生布局](halo/halo-room-ablation.md) · 初读挂点
- [异步前缀接续影响是否能坐下](halo/halo-rtc-ablation.md) · 初读挂点
- [流模型与回归的差异含RTC兼容性](halo/halo-decoder-ablation.md) · 初读挂点
- [技能库、视野与跟踪误差仍限定能力](halo/halo-limits.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
