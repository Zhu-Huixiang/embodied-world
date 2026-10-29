# 论文解读日程

正式系列沿具身榜高位向下精讲。Holo-M 留作试水稿。每日上海10:00启动精读与GitHub同步；日期是编辑目标，完成取决于审校与配图。当日已完成的解读占用当天名额，之后按未完成队列排期；历史完整解读保留在总队列。

| 拟定日期（上海） | 论文 / 榜单名次 | 本篇要讲清什么 | 实际进度 |
| --- | --- | --- | --- |
| 2026-10-30 | [Latent Diffusion · #3](../articles/latent-diffusion-2112.10752/README.md) | 为什么视频或图像模型常先压到 latent 空间，压缩省掉什么、又可能丢掉什么？ | 完整解读已审校 |
| 2026-10-30 | [ViT · #4](../articles/vit-2010.11929/README.md) | 一张图怎样变成 token 序列，机器人策略拿到的视觉特征来自哪一步？ | 完整解读已审校 |
| 2026-10-30 | [SAM · #5](../articles/sam-2304.02643/README.md) | 给视觉系统一个点或框，它怎样找到目标轮廓，哪些信息还需要控制策略来补？ | 完整解读已审校 |
| 2026-10-30 | [MAE · #6](../articles/mae-2111.06377/README.md) | 遮住四分之三的图像后还原像素，怎样帮助机器人把预训练视觉特征用于控制？ | 完整解读已审校 |
| 2026-10-30 | [MuZero · #7](../articles/muzero-1911.08265/README.md) | 用于规划的世界模型，为什么可以只预测奖励、价值和策略，而不重建下一帧？ | 完整解读已审校 |
| 2026-10-30 | [Attention Is All You Need · #8](../articles/attention-1706.03762/README.md) | Q、K、V 到底在计算什么，为什么这套序列计算能连接视觉、语言和动作？ | 完整解读已审校 |
| 2026-10-30 | [Emerging Properties in Self-Supervised Vision Transformers · #9](../articles/dino-2104.14294/README.md) | 没有人工标签，教师与学生互相对齐怎么还能长出物体边界？ | 完整解读已审校 |
| 2026-10-30 | [3D Gaussian Splatting for Real-Time Radiance Field Rendering · #10](../articles/gaussian-splatting-2308.04079/README.md) | 把神经场换成一群可编辑高斯，为什么渲染会快，场景操作又会方便在哪里？ | 完整解读已审校 |
| 2026-10-30 | [Scalable Diffusion Models with Transformers · #11](../articles/dit-2212.09748/README.md) | Transformer 怎样在潜空间去噪，条件又怎样进入各层？ | 完整解读已审校 |
| 2026-10-30 | [Diffusion Policy: Visuomotor Policy Learning via Action Diffusion · #12](../articles/diffusion-policy-2303.04137/README.md) | 为什么要对一段动作分布去噪，再滚动执行？ | 完整解读已审校 |
| 2026-10-30 | [NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis · #13](../articles/nerf-2003.08934/README.md) | 多张照片怎样变成可以换视角查看的场景，射线上每个采样点算了什么？ | 完整解读已审校 |
| 2026-10-30 | [Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware · #14](../articles/act-2304.13705/README.md) | Action chunking 与时间集成怎样处理示范中的误差累积？ | 完整解读已审校 |
| 2026-10-30 | [Mastering diverse control tasks through world models · #15](../articles/dreamerv3-2301.04104/README.md) | 跨任务尺度变化时，表征、价值和优化怎样保持可用？ | 完整解读已审校 |
| 2026-10-30 | [RT-1: Robotics Transformer for Real-World Control at Scale · #16](../articles/rt1-2212.06817/README.md) | 大量真实机器人数据究竟需要什么策略结构才能吃进去，TokenLearner 为何是关键？ | 完整解读已审校 |
| 2026-10-30 | [SAM 2: Segment Anything in Images and Videos · #17](../articles/sam2-2408.00714/README.md) | 目标在机器人视野里移动、遮挡后重现，过去的掩码记忆怎样帮它跟住对象？ | 完整解读已审校 |
| 2026-10-31 | [RMA: Rapid Motor Adaptation for Legged Robots · #18](../library/rma.md) | 训练时的环境特权信息，怎样通过历史状态在部署时估计？ | 机制初读，全文待制作 |
| 2026-11-01 | [DINOv2: Learning Robust Visual Features without Supervision · #19](../library/dinov2.md) | 机器人视觉编码器冻结以后，哪些几何和语义信息还能留在 patch 特征里？ | 机制初读，全文待制作 |
| 2026-11-02 | [Learning robust perceptive locomotion for quadrupedal robots in the wild · #20](../library/perceptive-loco.md) | 感知不可靠时，地形信息和本体反馈怎样共同支持行走？ | 机制初读，全文待制作 |
| 2026-11-03 | [Universal Manipulation Interface: In-The-Wild Robot Teaching Without In-The-Wild Robots · #21](../library/umi.md) | 拿手持夹爪采示范，怎样跨过人类手速、机器人延迟和坐标系之间的鸿沟？ | 机制初读，全文待制作 |
| 2026-11-04 | [Conservative Q-Learning for Offline Reinforcement Learning · #22](../library/cql.md) | 离线数据没有覆盖的动作，怎样避免被 Q 函数凭空吹成好动作？ | 机制初读，全文待制作 |
| 2026-11-05 | [DeepMimic: Example-Guided Deep Reinforcement Learning of Physics-Based Character Skills · #23](../library/deepmimic.md) | 模仿奖励与任务奖励怎样把动作片段变成可恢复的控制技能？ | 机制初读，全文待制作 |

[完整精讲队列](queue.md) · [具身榜](../leaderboard/README.md) · [论文地图](../paper-map/README.md) · [首页](../README.md)

选题快照：2026-10-10。
