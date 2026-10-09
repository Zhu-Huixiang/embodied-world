# 具身智能论文地图

从研究问题找论文：先看动作怎样表示，再看数据怎样监督，最后看策略怎样在闭环里执行。首批 30 篇同时构成后续解读的候选路线。

**三条起步路线**

- 动作生成：ACT → Diffusion Policy → FAST → π₀ / OpenVLA → Holo-M。
- 预测与控制：Dreamer → DreamerV2 / V3 → TD-MPC / TD-MPC2 → Cosmos Policy / DreamZero。
- 全身运动：DeepMimic → AMP → ASE；环境适应另走 RMA → DreamWaQ → Perceptive Locomotion。

箭头表示建议阅读次序，具体继承关系在逐篇解读中讨论。视频、图像生成和物理角色论文保留其原始任务范围。

## 世界模型与模型强化学习

未来状态怎样成为价值、策略或规划的训练场？

| 论文 / 出处 | 带着什么问题读 |
| --- | --- |
| [Dream to Control](../library/dreamer.md) · ICLR 2020 | RSSM 如何从观测和动作建模未来，actor 又怎样在潜空间学习？ |
| [Mastering Atari with Discrete World Models](../library/dreamerv2.md) · ICLR 2021 | 离散潜变量怎样帮助世界模型预测和想象？ |
| [Mastering diverse control tasks through world models](../library/dreamerv3.md) · Nature 2025 | 跨任务尺度变化时，表征、价值和优化怎样保持可用？ |
| [Temporal Difference Learning for Model Predictive Control](../library/td-mpc.md) · ICML 2022 | 怎样学习足够用于控制的潜动力学，而省去图像重建？ |
| [TD-MPC2](../library/td-mpc2.md) · ICLR 2024 | 多任务潜空间规划怎样处理不同动作空间和奖励尺度？ |

## 世界动作模型

视频与动作联合建模，怎样把预测变成执行？

| 论文 / 出处 | 带着什么问题读 |
| --- | --- |
| [World Action Models are Zero-shot Policies](../library/dreamzero.md) · arXiv 2026 | 视频与动作共同预测，怎样支持未见任务中的控制？ |
| [Cosmos Policy](../library/cosmos-policy.md) · arXiv 2026 | 视频生成序列怎样容纳动作、未来状态与规划信号？ |

## 视频动作模型与视觉推理

未来画面、动作和当前观测怎样相互约束？

| 论文 / 出处 | 带着什么问题读 |
| --- | --- |
| [CoT-VLA](../library/cot-vla.md) · CVPR 2025 | 预测未来图像作为目标，怎样帮助随后的一小段动作？ |
| [Causal World Modeling for Robot Control](../library/lingbot-va.md) · arXiv 2026 | 因果式视频与动作生成怎样缩小训练和闭环执行的差距？ |
| [VideoVLA](../library/videovla.md) · NeurIPS 2025 | 视频生成先验怎样与动作预测一起用于操作泛化？ |

## 视觉语言动作模型 VLA

视觉语言知识怎样接入动作表示、生成与训练？

| 论文 / 出处 | 带着什么问题读 |
| --- | --- |
| [Holo-M](../library/holo-m.md) · arXiv 2026 | 固定长度动作词表怎样同时连接跨来源数据和控制时钟？ |
| [FAST](../library/fast.md) · RSS 2025 | 为什么在时间频率域压缩，比逐时刻分箱更适合高频动作？ |
| [π₀](../library/pi0.md) · RSS 2025 | Flow Matching 动作专家怎样接收视觉语言条件？ |
| [OpenVLA](../library/openvla.md) · CoRL 2024 | 视觉特征融合、动作分箱和高效适配各自解决哪一层问题？ |
| [RT-2](../library/rt2.md) · CoRL 2023 | 文字和动作一起训练，网络知识怎样影响一次操作？ |
| [π₀.₅](../library/pi05.md) · arXiv 2025 | 跨本体、跨场景数据怎样变成开放环境中的长程操作？ |

## 操作与动作块

多模态动作分布、时间集成与执行延迟怎样影响接触？

| 论文 / 出处 | 带着什么问题读 |
| --- | --- |
| [Diffusion Policy](../library/diffusion-policy.md) · RSS 2023 | 为什么要对一段动作分布去噪，再滚动执行？ |
| [ACT](../library/act.md) · RSS 2023 | Action chunking 与时间集成怎样处理示范中的误差累积？ |
| [DP3](../library/dp3.md) · RSS 2024 | 简洁点云表示怎样改变操作策略的泛化？ |
| [Consistency Policy](../library/consistency-policy.md) · RSS 2024 | 蒸馏怎样减少去噪步骤，保留怎样的动作分布？ |

## Locomotion 与运动适应

看不全环境时，历史、本体与感知怎样支撑移动？

| 论文 / 出处 | 带着什么问题读 |
| --- | --- |
| [RMA](../library/rma.md) · RSS 2021 | 训练时的环境特权信息，怎样通过历史状态在部署时估计？ |
| [DreamWaQ](../library/dreamwaq.md) · ICRA 2023 | 盲行走时，历史本体信息怎样形成环境表征并进入 actor？ |
| [Learning robust perceptive locomotion for quadrupedal robots in the wild](../library/perceptive-loco.md) · Science-Robotics 2022 | 感知不可靠时，地形信息和本体反馈怎样共同支持行走？ |
| [Learning high-speed flight in the wild](../library/agile-flight.md) · Science-Robotics 2021 | 高速运动中的视觉规划，怎样跨越仿真与真实环境？ |

## 动作先验与全身技能

动作数据怎样变成可组合、可恢复的控制能力？

| 论文 / 出处 | 带着什么问题读 |
| --- | --- |
| [DeepMimic](../library/deepmimic.md) · SIGGRAPH-TOG 2018 | 模仿奖励与任务奖励怎样把动作片段变成可恢复的控制技能？ |
| [AMP](../library/amp.md) · SIGGRAPH-TOG 2021 | 判别器学到的动作先验，怎样替代逐帧跟踪奖励？ |
| [ASE](../library/ase.md) · SIGGRAPH-TOG 2022 | 连续技能潜变量怎样组织可重复使用的动作？ |

## 视频与序列生成

长序列滚动中的因果、噪声与误差积累怎样处理？

| 论文 / 出处 | 带着什么问题读 |
| --- | --- |
| [Diffusion Forcing](../library/diffusion-forcing.md) · NeurIPS 2024 | 各时间步不同噪声强度，怎样连接因果预测与整序列去噪？ |
| [Self Forcing](../library/self-forcing.md) · NeurIPS 2025 | 用模型自己滚出的历史训练，怎样处理自回归误差累积？ |

## Diffusion / Transformer 基础

去噪网络、条件注入与计算规模怎样影响表示？

| 论文 / 出处 | 带着什么问题读 |
| --- | --- |
| [DIT](../library/dit.md) · ICCV 2023 | Transformer 怎样在潜空间去噪，条件又怎样进入各层？ |

## 接下来怎样扩展

每次选题同时扫近期 arXiv、作者项目页与正式刊会目录；优先补齐一条路线中的关键机制、直接对照和新证据。新版本合并到已有卡片。候选卡片与已完成解读分别记录，周日程列出近期计划。

[全部论文元数据](../library/papers.json) · [顶会顶刊](../venues/README.md) · [未来一周](../calendar/README.md) · [首页](../README.md)

元数据核对日期：2026-10-09。

<!-- discovery:start -->
## 新作阅读支路

- [Dex-One2Many: Learning Dexterous Manipulation from a Single Human Demonstration](../library/dex-one2many.md)：场景图怎样同时提供探索引导与不锁死姿态的泛化？
- [DreamTrue: Action-Faithful Robot World Model with Counterfactual Post-Training](../library/dreamtrue.md)：模型怎样避免把每次接触都预测成成功？
- [A Balanced Data Diet: Addressing the Exploration Bottleneck in Mega-Scale RL for Robot Control](../library/balanced-data-diet.md)：并行环境堆到很大以后，为什么探索还会卡住？
- [VioLA: Learning Generalist Humanoid Control Policies from Human Data](../library/viola.md)：人类动作怎样先对齐控制器，再教会人形 VLA？
- [LeWAM: A JEPA World Action Model with Diffusion-Steering-Based MPC](../library/lewam.md)：联合表征怎样支持预测、动作生成和闭环规划？
- [ARC: A Reasoning Recipe for Robot Foundation Models](../library/arc.md)：推理文字怎样成为动作条件，而不是另一段好看的解说？
- [PLaW-VLA: Predictive Latent World Modeling for Vision-Language-Action Policies](../library/plaw-vla.md)：怎样证明预测的未来表征真的帮助长程动作？

[按日期追新作](../arxiv/README.md) · [六维阅读优先榜](../leaderboard/README.md)
<!-- discovery:end -->
