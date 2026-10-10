# 具身智能论文地图

从研究问题找论文：动作怎样表示、数据怎样监督、策略怎样闭环执行。正式系列按[具身榜](../leaderboard/README.md)顺序精讲；这里按问题组织阅读支路。含 108 篇已核验论文，另有[arXiv新作](../arxiv/README.md)。

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
| [Mastering Atari Games with Limited Data](../library/efficientzero.md) · NeurIPS 2021 | 只有少量交互时，潜空间树搜索为什么还需要一致性监督、价值前缀和重分析？ |
| [EfficientZero V2](../library/efficientzero-v2.md) · ICML 2024 | 树搜索怎样跨过离散动作的限制，在连续控制里仍保持样本效率？ |
| [DayDreamer](../library/daydreamer.md) · CoRL 2022 | 世界模型的想象训练怎样接到真实机器人持续在线交互上？ |
| [Offline Reinforcement Learning as One Big Sequence Modeling Problem](../library/trajectory-transformer.md) · NeurIPS 2021 | 状态、动作和奖励一起变成 token 后，beam search 为什么可以用来规划？ |
| [Mastering Atari, Go, chess and shogi by planning with a learned model](../library/muzero.md) · Nature 2020 | 用于规划的世界模型，为什么可以只预测奖励、价值和策略，而不重建下一帧？ |
| [LeWorldModel](../library/lewm.md) · arXiv 2026 | 两项损失怎样让像素JEPA不坍缩，又把每帧压成一个可规划的token？ |
| [Ctrl-World](../library/ctrl-world.md) · ICLR 2026 | 怎样让视频生成器按真实动作走，并使想象中的策略排名接近实机？ |
| [A review of learning-based dynamics models for robotic manipulation](../library/learned-dynamics-review.md) · Science-Robotics 2025 | 世界模型该预测像素、latent、粒子还是物体？换种表示会怎样改写感知与规划的代价？ |
| [V-JEPA 2](../library/vjepa2.md) · arXiv 2025 | 先看无动作标签视频，再给少量机器人交互，潜空间怎样变成 Franka 规划器？ |

## 世界动作模型

视频与动作联合建模，怎样把预测变成执行？

| 论文 / 出处 | 带着什么问题读 |
| --- | --- |
| [World Action Models are Zero-shot Policies](../library/dreamzero.md) · arXiv 2026 | 视频与动作共同预测，怎样支持未见任务中的控制？ |
| [Cosmos Policy](../library/cosmos-policy.md) · ICLR 2026 | 视频生成序列怎样容纳动作、未来状态与规划信号？ |
| [Planning with Diffusion for Flexible Behavior Synthesis](../library/diffuser.md) · ICML 2022 | 轨迹一起去噪，如何同时承担环境建模、长时序规划与测试时加约束？ |
| [Modality-Autoregressive World-Action Models](../library/modar.md) · arXiv 2026 | 为什么先预测点轨迹、语义与几何，再给动作，可能比视频动作一起去噪更有效？ |

## 视频动作模型与视觉推理

未来画面、动作和当前观测怎样相互约束？

| 论文 / 出处 | 带着什么问题读 |
| --- | --- |
| [CoT-VLA](../library/cot-vla.md) · CVPR 2025 | 预测未来图像作为目标，怎样帮助随后的一小段动作？ |
| [Causal World Modeling for Robot Control](../library/lingbot-va.md) · RSS 2026 | 视频预测具体给动作带来什么，真实反馈怎样写回KV历史，又怎样少去噪而保住控制质量？ |
| [VideoVLA](../library/videovla.md) · NeurIPS 2025 | 视频生成先验怎样与动作预测一起用于操作泛化？ |
| [Learning Universal Policies via Text-Guided Video Generation](../library/unipi.md) · NeurIPS 2023 | 先生成机器人会怎么做的视频，再倒推出动作，这条路线解决了什么又把难题搬到了哪里？ |

## 视觉语言动作模型 VLA

视觉语言知识怎样接入动作表示、生成与训练？

| 论文 / 出处 | 带着什么问题读 |
| --- | --- |
| [Holo-M](../library/holo-m.md) · arXiv 2026 | 固定长度动作词表怎样同时连接跨来源数据和控制时钟？ |
| [FAST](../library/fast.md) · RSS 2025 | 为什么在时间频率域压缩，比逐时刻分箱更适合高频动作？ |
| [π₀](../library/pi0.md) · RSS 2025 | Flow Matching 动作专家怎样接收视觉语言条件？ |
| [OpenVLA](../library/openvla.md) · CoRL 2024 | 视觉特征融合、动作分箱和高效适配各自解决哪一层问题？ |
| [RT-2](../library/rt2.md) · CoRL 2023 | 文字和动作一起训练，网络知识怎样影响一次操作？ |
| [π₀.₅](../library/pi05.md) · CoRL 2025 | 跨本体、跨场景数据怎样变成开放环境中的长程操作？ |
| [RT-1](../library/rt1.md) · RSS 2023 | 大量真实机器人数据究竟需要什么策略结构才能吃进去，TokenLearner 为何是关键？ |
| [Do As I Can, Not As I Say](../library/saycan.md) · CoRL 2022 | 语言模型觉得该做的事，机器人做得到吗？两个概率相乘到底解决什么？ |
| [PaLM-E](../library/palm-e.md) · ICML 2023 | 把传感器读数塞进语言模型的 embedding 空间，能带来怎样的机器人推理？ |
| [Open X-Embodiment](../library/rtx.md) · ICRA 2024 | 不同机器人的动作坐标和观测并不一致，怎样把它们混成能产生正迁移的数据？ |
| [Octo](../library/octo.md) · RSS 2024 | 通用策略接上新摄像头、新动作空间时，哪些模块可以保留，哪些需要改？ |
| [VIMA](../library/vima.md) · ICML 2023 | 文字、目标图和示范视频能否作为同一种任务提示交给机器人？ |
| [GR00T N1](../library/gr00t-n1.md) · arXiv 2025 | Eagle-2视觉语言特征与连续动作流怎样分工，合成视频里的动作标签从哪来，预训练收益又在什么任务上成立？ |

## 操作与动作块

多模态动作分布、时间集成与执行延迟怎样影响接触？

| 论文 / 出处 | 带着什么问题读 |
| --- | --- |
| [Diffusion Policy](../library/diffusion-policy.md) · RSS 2023 | 为什么要对一段动作分布去噪，再滚动执行？ |
| [ACT](../library/act.md) · RSS 2023 | Action chunking 与时间集成怎样处理示范中的误差累积？ |
| [DP3](../library/dp3.md) · RSS 2024 | 简洁点云表示怎样改变操作策略的泛化？ |
| [Consistency Policy](../library/consistency-policy.md) · RSS 2024 | 蒸馏怎样减少去噪步骤，保留怎样的动作分布？ |
| [CLIPort](../library/cliport.md) · CoRL 2021 | CLIP 知道是什么，但不知道手该落在哪里；语义和几何怎样配合？ |
| [Perceiver-Actor](../library/peract.md) · CoRL 2022 | 把动作当成体素中的检测目标，为什么比从整张图片直接回归动作更省示范？ |
| [RVT](../library/rvt.md) · CoRL 2023 | 体素太贵，重渲染几张虚拟视图能保住 3D 信息吗？ |
| [RVT-2](../library/rvt2.md) · RSS 2024 | 粗视图定位之后再放大，怎样改善毫米级插入，而不是只让网络更快？ |
| [What Matters in Learning from Offline Human Demonstrations for Robot Manipulation](../library/robomimic.md) · CoRL 2021 | 同样的人类示范，为什么换个观测历史、数据质量或停训方式，结果会差这么多？ |
| [BridgeData V2](../library/bridge-v2.md) · CoRL 2023 | 机器人数据怎样覆盖场景差异，才会支持跨环境与跨机构技能迁移？ |
| [DROID](../library/droid.md) · RSS 2024 | 机器人长期困在少数桌面场景里，分布式真实数据能把泛化边界推远多少？ |
| [LIBERO](../library/libero.md) · NeurIPS 2023 | 一个机器人顺序学新任务时，究竟迁移的是物体概念、动作技能，还是两者的组合？ |
| [RoboCasa](../library/robocasa.md) · RSS 2024 | 真实数据太贵，家居仿真的场景、任务与示范各要扩到什么程度才有用？ |
| [Mobile ALOHA](../library/mobile-aloha.md) · CoRL 2024 | 桌面双臂经验为什么能帮会移动的机器人做饭、开柜子和坐电梯？ |
| [Universal Manipulation Interface](../library/umi.md) · RSS 2024 | 拿手持夹爪采示范，怎样跨过人类手速、机器人延迟和坐标系之间的鸿沟？ |
| [MimicGen](../library/mimicgen.md) · CoRL 2023 | 把十条示范扩成上千条，什么时候是有用的新数据，什么时候只是机械复制？ |
| [Behavior Generation with Latent Actions](../library/vq-bet.md) · ICML 2024 | 动作先压成分层离散码，能否保留多种操作方式，同时省掉扩散反复采样？ |
| [Transporter Networks](../library/transporter.md) · CoRL 2020 | 操作物体不一定要先识别物体？空间特征之间的匹配怎么直接长出动作？ |
| [EgoScale](../library/egoscale.md) · arXiv 2026 | 人类视频怎样变成机器人可学的手腕和手指动作，为什么大量预训练之后还要一小段人机对齐数据？ |

## Locomotion 与运动适应

看不全环境时，历史、本体与感知怎样支撑移动？

| 论文 / 出处 | 带着什么问题读 |
| --- | --- |
| [RMA](../library/rma.md) · RSS 2021 | 训练时的环境特权信息，怎样通过历史状态在部署时估计？ |
| [DreamWaQ](../library/dreamwaq.md) · ICRA 2023 | 盲行走时，历史本体信息怎样形成环境表征并进入 actor？ |
| [Learning robust perceptive locomotion for quadrupedal robots in the wild](../library/perceptive-loco.md) · Science-Robotics 2022 | 感知不可靠时，地形信息和本体反馈怎样共同支持行走？ |
| [Learning high-speed flight in the wild](../library/agile-flight.md) · Science-Robotics 2021 | 高速运动中的视觉规划，怎样跨越仿真与真实环境？ |
| [Learning to Walk in Minutes Using Massively Parallel Deep Reinforcement Learning](../library/walk-in-minutes.md) · CoRL 2021 | 把几千只机器人放到同一块 GPU，训练速度与课程怎么一起改变？ |
| [Walk These Ways](../library/walk-these-ways.md) · CoRL 2022 | 遇到新地面不重训，能否直接调一组步态参数让同一个策略换种走法？ |
| [Extreme Parkour with Legged Robots](../library/extreme-parkour.md) · ICRA 2024 | 低频深度相机和不精确电机，怎样还能触发踩点精确的跳跃？ |
| [ANYmal parkour](../library/anymal-parkour.md) · Science-Robotics 2024 | 会跳、会爬的低层技能，怎样被高层导航策略排成一条可走路线？ |
| [Learning agile soccer skills for a bipedal robot with deep reinforcement learning](../library/bipedal-soccer.md) · Science-Robotics 2024 | 踢球、摔倒再爬起和防守，怎样被训练成会连续切换的全身行为？ |
| [HumanPlus](../library/humanplus.md) · CoRL 2024 | 人做动作、机器人跟动作、再学自主任务，这三段数据链路如何接起来？ |
| [OmniH2O](../library/omnih2o.md) · CoRL 2024 | 只有头和双手目标，为什么还能指挥整个身体并收集自主学习数据？ |
| [ASAP](../library/asap.md) · RSS 2025 | 模拟和实机差一点，为什么补动作残差比盲目加大随机化更有针对性？ |
| [Deep Whole-Body Control](../library/deep-whole-body-control.md) · CoRL 2022 | 手臂和腿一起出动作，怎样避免一边拿东西、一边把身体拽倒？ |
| [Expressive Whole-Body Control for Humanoid Robots](../library/exbody.md) · RSS 2024 | 上半身想照着人动，下半身还得站稳，这两种目标怎么兼容？ |
| [Demonstrating A Walk in the Park](../library/walk-in-the-park.md) · RSS 2023 | 没有世界模型和动作模板，如何把实机采样与梯度更新快到足够实用？ |
| [SONIC](../library/sonic.md) · Science-Robotics 2026 | 动作跟踪为什么能吃进大规模人类动作数据，64维共享运动 token 又怎样让同一控制器接遥操作和全身 VLA？ |
| [HOVER](../library/hover.md) · ICRA 2025 | 一个全身策略怎样接住关节、身体位置、根速度等不同格式的指令？ |

## 动作先验与全身技能

动作数据怎样变成可组合、可恢复的控制能力？

| 论文 / 出处 | 带着什么问题读 |
| --- | --- |
| [DeepMimic](../library/deepmimic.md) · SIGGRAPH-TOG 2018 | 模仿奖励与任务奖励怎样把动作片段变成可恢复的控制技能？ |
| [AMP](../library/amp.md) · SIGGRAPH-TOG 2021 | 判别器学到的动作先验，怎样替代逐帧跟踪奖励？ |
| [ASE](../library/ase.md) · SIGGRAPH-TOG 2022 | 连续技能潜变量怎样组织可重复使用的动作？ |
| [MaskedMimic](../library/maskedmimic.md) · SIGGRAPH-TOG 2024 | 把动作目标遮掉一部分，怎样训练出接受位置、文字和环境条件的统一控制器？ |
| [Perpetual Humanoid Control for Real-time Simulated Avatars](../library/phc.md) · ICCV 2023 | 动作库越来越大，跟踪控制器怎样扩容、处理噪声并在摔倒后接着跑？ |

## 强化学习与离线决策

奖励、价值估计与数据覆盖怎样决定策略能学到什么？

| 论文 / 出处 | 带着什么问题读 |
| --- | --- |
| [Offline Reinforcement Learning with Implicit Q-Learning](../library/iql.md) · ICLR 2022 | 从未评价数据外动作，IQL 为什么还能拼接次优轨迹并改善策略？ |
| [A Minimalist Approach to Offline Reinforcement Learning](../library/td3-bc.md) · NeurIPS 2021 | 只在 TD3 策略损失里加一个模仿项，为什么能成为可靠的离线 RL 基线？ |
| [Decision Transformer](../library/decision-transformer.md) · NeurIPS 2021 | 把目标回报放进 token 序列，就能把离线控制改写成条件生成吗？ |
| [Cal-QL](../library/cal-ql.md) · NeurIPS 2023 | 离线训练把 Q 压得太低，为什么一上真环境反而会先忘掉已有技能？ |
| [Conservative Q-Learning for Offline Reinforcement Learning](../library/cql.md) · NeurIPS 2020 | 离线数据没有覆盖的动作，怎样避免被 Q 函数凭空吹成好动作？ |
| [Isaac Gym](../library/isaac-gym.md) · NeurIPS-Datasets-Benchmarks 2021 | GPU 仿真、奖励和策略更新怎样连成一条流水线，改变机器人 RL 的试错速度？ |

## 具身感知与场景表示

视觉表征、几何与语言怎样给机器人提供可用的状态？

| 论文 / 出处 | 带着什么问题读 |
| --- | --- |
| [R3M](../library/r3m.md) · CoRL 2022 | 人类第一视角视频里学来的视觉表征，怎样成为机器人少样本操作的感知模块？ |
| [VIP](../library/vip.md) · ICLR 2023 | 两张图在 latent 空间的距离，为什么可以变成机器人离目标还有多远的奖励？ |
| [Where are we in the search for an Artificial Visual Cortex for Embodied Intelligence?](../library/vc1.md) · NeurIPS 2023 | 有没有一套视觉编码器在所有具身任务上都强？扩大人类视频数据就够了吗？ |
| [An Image is Worth 16x16 Words](../library/vit.md) · ICLR 2021 | 一张图怎样变成 token 序列，机器人策略拿到的视觉特征来自哪一步？ |
| [Learning Transferable Visual Models From Natural Language Supervision](../library/clip.md) · ICML 2021 | 图像和一句指令怎样对齐，语义相似为什么还不能直接给出抓取位置？ |
| [Emerging Properties in Self-Supervised Vision Transformers](../library/dino.md) · ICCV 2021 | 没有人工标签，教师与学生互相对齐怎么还能长出物体边界？ |
| [DINOv2](../library/dinov2.md) · TMLR 2024 | 机器人视觉编码器冻结以后，哪些几何和语义信息还能留在 patch 特征里？ |
| [Masked Autoencoders Are Scalable Vision Learners](../library/mae.md) · CVPR 2022 | 遮住四分之三的图像后还原像素，怎样帮助机器人把预训练视觉特征用于控制？ |
| [Segment Anything](../library/sam.md) · ICCV 2023 | 给视觉系统一个点或框，它怎样找到目标轮廓，哪些信息还需要控制策略来补？ |
| [SAM 2](../library/sam2.md) · ICLR 2025 | 目标在机器人视野里移动、遮挡后重现，过去的掩码记忆怎样帮它跟住对象？ |
| [NeRF](../library/nerf.md) · ECCV 2020 | 多张照片怎样变成可以换视角查看的场景，射线上每个采样点算了什么？ |
| [3D Gaussian Splatting for Real-Time Radiance Field Rendering](../library/gaussian-splatting.md) · SIGGRAPH-TOG 2023 | 把神经场换成一群可编辑高斯，为什么渲染会快，场景操作又会方便在哪里？ |
| [Self-Supervised Learning from Images with a Joint-Embedding Predictive Architecture](../library/i-jepa.md) · CVPR 2023 | 世界模型必须把像素画出来吗，预测目标区域的 latent 会保留哪些可用信息？ |

## 视频与序列生成

长序列滚动中的因果、噪声与误差积累怎样处理？

| 论文 / 出处 | 带着什么问题读 |
| --- | --- |
| [Diffusion Forcing](../library/diffusion-forcing.md) · NeurIPS 2024 | 各时间步不同噪声强度，怎样连接因果预测与整序列去噪？ |
| [Self Forcing](../library/self-forcing.md) · NeurIPS 2025 | 用模型自己滚出的历史训练，怎样处理自回归误差累积？ |
| [Video Diffusion Models](../library/video-diffusion.md) · NeurIPS 2022 | 逐帧画图为什么会抖，空间与时间注意力怎样让一段未来视频连起来？ |
| [Phenaki](../library/phenaki.md) · ICLR 2023 | 一段视频怎样变成短 token 序列，因果编码又怎样允许它继续往后生成？ |

## Diffusion / Transformer 基础

去噪网络、条件注入与计算规模怎样影响表示？

| 论文 / 出处 | 带着什么问题读 |
| --- | --- |
| [DIT](../library/dit.md) · ICCV 2023 | Transformer 怎样在潜空间去噪，条件又怎样进入各层？ |
| [Attention Is All You Need](../library/attention.md) · NeurIPS 2017 | Q、K、V 到底在计算什么，为什么这套序列计算能连接视觉、语言和动作？ |
| [Denoising Diffusion Probabilistic Models](../library/ddpm.md) · NeurIPS 2020 | 加噪声再预测噪声的训练目标，怎样变成一段机器人动作的采样算法？ |
| [Denoising Diffusion Implicit Models](../library/ddim.md) · ICLR 2021 | 去噪训练目标不变，为什么推理时能跳步，延迟与样本质量该怎样交换？ |
| [High-Resolution Image Synthesis with Latent Diffusion Models](../library/latent-diffusion.md) · CVPR 2022 | 为什么视频或图像模型常先压到 latent 空间，压缩省掉什么、又可能丢掉什么？ |
| [Elucidating the Design Space of Diffusion-Based Generative Models](../library/edm.md) · NeurIPS 2022 | 同样是扩散，噪声尺度、网络预处理和数值求解器各改变了哪一层？ |
| [Flow Matching for Generative Modeling](../library/flow-matching.md) · ICLR 2023 | 不模拟整条生成轨迹就能训练速度场，π₀ 里的 Flow Matching 损失怎样读？ |
| [Flow Straight and Fast](../library/rectified-flow.md) · ICLR 2023 | 训练速度场和把轨迹拉直有什么区别，为什么直一点就能少算几步？ |
| [Consistency Models](../library/consistency-models.md) · ICML 2023 | 沿同一条去噪轨迹的不同点，怎样被一个模型直接映射回同一样本？ |

[高影响论文收录清单与筛选依据](curated-2026-10-10.md) · [全部论文元数据](../library/papers.json) · [顶会顶刊](../venues/README.md) · [未来一周](../calendar/README.md) · [首页](../README.md)

元数据核对日期：2026-10-10。

<!-- discovery:start -->
## 新作阅读支路

- [Dex-One2Many: Learning Dexterous Manipulation from a Single Human Demonstration](../library/dex-one2many.md)：场景图怎样同时提供探索引导与不锁死姿态的泛化？
- [DreamTrue: Action-Faithful Robot World Model with Counterfactual Post-Training](../library/dreamtrue.md)：模型怎样避免把每次接触都预测成成功？
- [A Balanced Data Diet: Addressing the Exploration Bottleneck in Mega-Scale RL for Robot Control](../library/balanced-data-diet.md)：并行环境堆到很大以后，为什么探索还会卡住？
- [VioLA: Learning Generalist Humanoid Control Policies from Human Data](../library/viola.md)：人类动作怎样先对齐控制器，再教会人形 VLA？
- [LeWAM: A JEPA World Action Model with Diffusion-Steering-Based MPC](../library/lewam.md)：联合表征怎样支持预测、动作生成和闭环规划？
- [ARC: A Reasoning Recipe for Robot Foundation Models](../library/arc.md)：推理文字怎样成为动作条件，而不是另一段好看的解说？
- [PLaW-VLA: Predictive Latent World Modeling for Vision-Language-Action Policies](../library/plaw-vla.md)：怎样证明预测的未来表征真的帮助长程动作？

[按日期追新作](../arxiv/README.md) · [七维阅读优先榜](../leaderboard/README.md)
<!-- discovery:end -->
