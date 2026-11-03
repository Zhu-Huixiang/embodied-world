# Perceptive Locomotion 星系

Learning robust perceptive locomotion for quadrupedal robots in the wild

**已精讲** · Locomotion 与运动适应

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md) · [原文](https://www.science.org/doi/10.1126/scirobotics.abk2822) · [评分卡](../../leaderboard/papers/perceptive-loco/README.md)

让地形感知与本体反馈共同支持腿足策略，在复杂户外地形中考察感知失效和控制鲁棒性。

## 技术挂点

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#44-观察与动作从-391-个数到-12-个关节目标)

- [环境适应](../concepts/adaptation.md)：根据历史观测或环境信息调整策略，使动力学或地形变化仍可处理。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#48-信念编码器门控与记忆分别做什么)

- [仿真到实机](../concepts/sim2real.md)：处理仿真动力学、感知和真实系统间的差异，通过随机化、辨识、残差或适配来迁移。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#49-部署20-hz-地图接上-50-hz-控制)

- [特权训练信息](../concepts/privileged.md)：训练用额外环境真值或教师信息，部署另用可获取输入估计或模仿。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#43-教师策略它先拿到哪些答案)

- [强化学习](../concepts/rl.md)：通过奖励和值评估改进策略，研究动作如何改变长期回报。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#43-教师策略它先拿到哪些答案)

- [PPO 与并行模拟](../concepts/ppo.md)：用受约束的策略更新与大量模拟轨迹训练控制；并行度改变每轮数据和训练开销。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#43-教师策略它先拿到哪些答案)

- [教师学生蒸馏](../concepts/distill.md)：用教师的预测分布、特征或动作监督学生，把已有模型的可用信息迁移到学生。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#46-学生训练模仿动作也重建环境)

- [示范模仿](../concepts/imitation.md)：从专家、人类或教师策略的行为学习动作，研究数据、表示和执行误差。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#46-学生训练模仿动作也重建环境)

- [行为克隆](../concepts/bc.md)：直接监督观测到动作的映射，不必在每次更新中根据奖励搜索。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#46-学生训练模仿动作也重建环境)

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#44-观察与动作从-391-个数到-12-个关节目标)

- [闭环滚动与历史偏移](../concepts/rollout.md)：重复预测、执行或生成，把新观测或模型历史接回后续计算。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#46-学生训练模仿动作也重建环境)

## 本篇行星与卫星

- [空间表示](perceptive-loco/spatial.md) · 已讲解
- [环境适应](perceptive-loco/adaptation.md) · 已讲解
- [仿真到实机](perceptive-loco/sim2real.md) · 已讲解
- [特权训练信息](perceptive-loco/privileged.md) · 已讲解
- [强化学习](perceptive-loco/rl.md) · 已讲解
- [PPO 与并行模拟](perceptive-loco/ppo.md) · 已讲解
- [教师学生蒸馏](perceptive-loco/distill.md) · 已讲解
- [示范模仿](perceptive-loco/imitation.md) · 已讲解
- [行为克隆](perceptive-loco/bc.md) · 已讲解
- [动作表示](perceptive-loco/action.md) · 已讲解
- [闭环滚动与历史偏移](perceptive-loco/rollout.md) · 已讲解
- [本篇方法链路](perceptive-loco/method-chain.md) · 已讲解
- [可靠地图是一个会失效的前提](perceptive-loco/method-map-assumption.md) · 已讲解
- [一次2.2公里的户外路线验证](perceptive-loco/experiment-hike.md) · 已讲解
- [多季节部署与零跌倒的范围](perceptive-loco/experiment-field-scope.md) · 已讲解
- [高度图错误有不同来源](perceptive-loco/method-map-failure.md) · 已讲解
- [2.5D地图只给每个平面位置一个高度](perceptive-loco/method-map-geometry.md) · 已讲解
- [脚滑会反过来弄坏地图](perceptive-loco/method-pose-map-coupling.md) · 已讲解
- [实机台阶成功率的十次试验](perceptive-loco/experiment-step-protocol.md) · 已讲解
- [线速度与转向速度分别比较](perceptive-loco/experiment-speed.md) · 已讲解
- [受辅助的障碍路线不作速度倍数](perceptive-loco/experiment-path-help.md) · 已讲解
- [软泡沫触地后向下修正内部地形](perceptive-loco/experiment-foam.md) · 已讲解
- [透明台阶接触后向上修正](perceptive-loco/experiment-transparent.md) · 已讲解
- [遮挡传感器后退回接触反应](perceptive-loco/experiment-blind.md) · 已讲解
- [摩擦曲线是内省解码结果](perceptive-loco/experiment-friction-decoding.md) · 已讲解
- [信念状态没有显式风险分布](perceptive-loco/limit-uncertainty.md) · 已讲解
- [高度图换来传感器兼容也丢掉外观](perceptive-loco/limit-sensor-abstraction.md) · 已讲解
- [用历史补足当下看不全的状态](perceptive-loco/method-pomdp.md) · 已讲解
- [特权教师、带噪学生、实机部署](perceptive-loco/method-three-stages.md) · 已讲解
- [仿真动力学与学习到的执行器模型](perceptive-loco/method-simulation.md) · 已讲解
- [用箱体楼梯堵住仿真几何捷径](perceptive-loco/method-stair-geometry.md) · 已讲解
- [随机化身体与接触条件](perceptive-loco/method-randomization.md) · 已讲解
- [不良状态触发训练终止](perceptive-loco/method-termination.md) · 已讲解
- [地形课程与代价课程分开推进](perceptive-loco/method-curriculum.md) · 已讲解
- [教师先用仿真真值学控制](perceptive-loco/method-privileged-teacher.md) · 已讲解
- [两路压缩后再接动作网络](perceptive-loco/method-teacher-latents.md) · 已讲解
- [每轮并行采样不等于总训练时长](perceptive-loco/method-training-budget.md) · 已讲解
- [391维教师输入与341维学生输入](perceptive-loco/method-observation-shapes.md) · 已讲解
- [每脚五圈共52个高度样本](perceptive-loco/method-height-rings.md) · 已讲解
- [接触与扰动真值只在训练侧可见](perceptive-loco/method-privileged-input.md) · 已讲解
- [16维动作经CPG与IK变成目标角](perceptive-loco/method-action-cpg.md) · 已讲解
- [名义摆腿轨迹是可修正的脚端基准](perceptive-loco/method-nominal-trajectory.md) · 已讲解
- [速度之外还惩罚滑动、碰撞与激烈动作](perceptive-loco/method-reward-tradeoffs.md) · 已讲解
- [足端离地过高也会受罚](perceptive-loco/method-clearance-cost.md) · 已讲解
- [在学生自己访问的状态上向教师学](perceptive-loco/method-student-rollout.md) · 已讲解
- [动作模仿与环境重建共同监督](perceptive-loco/method-two-losses.md) · 已讲解
- [沿用教师主网络来初始化学生](perceptive-loco/method-student-initialization.md) · 已讲解
- [把噪声加在位置、高度和不同时间范围](perceptive-loco/method-noise-scopes.md) · 已讲解
- [三种地图质量按60比30比10采样](perceptive-loco/method-noise-mixture.md) · 已讲解
- [学生先学简单地形再加大感知破坏](perceptive-loco/method-noise-curriculum.md) · 已讲解
- [截断梯度长度不是记忆保质期](perceptive-loco/method-truncated-gradient.md) · 已讲解
- [两层GRU积累接触与感知历史](perceptive-loco/method-recurrent-belief.md) · 已讲解
- [门控调节外感特征的捷径](perceptive-loco/method-gated-skip.md) · 已讲解
- [96维外感必须补到120维才能相加](perceptive-loco/method-zero-padding.md) · 已讲解
- [辅助解码器让内部表征有可检查目标](perceptive-loco/method-auxiliary-decoder.md) · 已讲解
- [20Hz地图与50Hz动作异步衔接](perceptive-loco/method-deployment-loops.md) · 已讲解
- [同一高度接口连接两种传感配置](perceptive-loco/method-sensor-variants.md) · 已讲解
- [地形参数网格上的仿真成功范围](perceptive-loco/experiment-simulation-grid.md) · 已讲解
- [用四种编码器分开检验记忆与门控](perceptive-loco/experiment-gate-ablation.md) · 已讲解
- [门控动作误差优势要逐条件读](perceptive-loco/experiment-action-error.md) · 已讲解
- [重建更准与行走成功分开验证](perceptive-loco/experiment-reconstruction-error.md) · 已讲解
- [每高度100次的仿真过阶消融](perceptive-loco/experiment-step-ablation.md) · 已讲解

## 论文间的联系

- [Perceptive Locomotion](perceptive-loco.md) → [RMA](rma.md)：引言将RMA列为已迁移到物理机器人的强化学习腿足方法之一；此关系表示原文引用，方法采用仍须另有证据。 [原文定位](https://leggedrobotics.github.io/rl-perceptiveloco/assets/pdf/wild_anymal.pdf)（§1, p3, reference[39]; bibliography p15）。

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
