# 知识点宇宙

[打开交互宇宙](https://zhu-huixiang.github.io/embodied-world/universe/) · [离线单文件](index.html) · [图谱数据](graph.json)

120 篇论文是恒星，各自有自己的知识行星与卫星：共 601 个本篇挂点，另外 59 个共享技术入口把星系连接起来。亮起的 2 篇有完整解读，59 个本篇挂点有具体章节讲解。暗星也能点击，进入机制导读和原文。

每篇保留初读已核概念和完整机制；已精讲论文逐章节补本篇知识点，未精讲星系随原文核验扩展，不声称初读覆盖全部附录。

搜索论文或知识点，按方向或亮度筛选。选中节点后可查看邻域、打开讲解；拖动空白平移，滚轮或按钮缩放。页面下方的节点列表支持键盘操作。

连线有三类：论文包含/讨论知识点；知识点的编辑分类层级；有原文定位的论文采用/引用。共享知识点只保留一个节点。层级用于导航，不宣称因果或学习先修顺序；共享技术不自动生成引用关系。

## 论文星系

| 论文 | 亮度 | 技术入口 |
| --- | --- | --- |
| [ACT / ALOHA](papers/act.md) | 导读 | [变分自编码器 VAE](concepts/vae.md) · [动作块](concepts/chunk.md) · [行为克隆](concepts/bc.md) |
| [Agile Flight](papers/agile-flight.md) | 导读 | [教师学生蒸馏](concepts/distill.md) · [仿真到实机](concepts/sim2real.md) · [空间表示](concepts/spatial.md) |
| [AMP](papers/amp.md) | 导读 | [对抗动作模仿](concepts/adversarial.md) · [动作先验](concepts/motion-prior.md) · [强化学习](concepts/rl.md) |
| [ANYmal Parkour](papers/anymal-parkour.md) | 导读 | [分层技能与计划](concepts/skills.md) · [空间表示](concepts/spatial.md) · [仿真到实机](concepts/sim2real.md) |
| [ARC](papers/arc.md) | 导读 | [因果序列建模](concepts/causal.md) · [动作表示](concepts/action.md) · [世界动作联合建模](concepts/wam.md) |
| [ASAP](papers/asap.md) | 导读 | [运动重定向](concepts/retarget.md) · [动作条件动力学](concepts/dynamics.md) · [仿真到实机](concepts/sim2real.md) |
| [ASE](papers/ase.md) | 导读 | [对抗动作模仿](concepts/adversarial.md) · [分层技能与计划](concepts/skills.md) · [表征空间](concepts/representation.md) |
| [Transformer](papers/attention.md) | 导读 | [注意力](concepts/attention.md) · [因果序列建模](concepts/causal.md) · [Transformer](concepts/transformer.md) |
| [Balanced Data Diet](papers/balanced-data-diet.md) | 导读 | [机器人数据与评测](concepts/data.md) · [强化学习](concepts/rl.md) · [教师学生蒸馏](concepts/distill.md) |
| [Bipedal Soccer](papers/bipedal-soccer.md) | 导读 | [策略与价值学习](concepts/actor-critic.md) · [分层技能与计划](concepts/skills.md) · [仿真到实机](concepts/sim2real.md) |
| [BridgeData V2](papers/bridge-v2.md) | 导读 | [行为克隆](concepts/bc.md) · [跨本体数据](concepts/cross-body.md) · [泛化评测与遗忘](concepts/benchmark.md) |
| [Cal-QL](papers/cal-ql.md) | 导读 | [离线强化学习](concepts/offline.md) · [价值估计与校准](concepts/value.md) · [策略与价值学习](concepts/actor-critic.md) |
| [CLIP](papers/clip.md) | 已精讲 | [对比学习](concepts/contrastive.md) · [向量归一化](concepts/normalization.md) · [余弦相似度](concepts/cosine.md) · [交叉熵](concepts/cross-entropy.md) · [softmax 与温度](concepts/softmax.md) · [视觉 patch token](concepts/patches.md) · [零样本任务接口](concepts/zero-shot.md) · [提示模板集成](concepts/prompt-ensemble.md) · [线性探测](concepts/linear-probe.md) · [分布偏移](concepts/shift.md) · [空间表示](concepts/spatial.md) |
| [CLIPort](papers/cliport.md) | 导读 | [对比学习](concepts/contrastive.md) · [空间表示](concepts/spatial.md) · [示范模仿](concepts/imitation.md) |
| [Consistency Models](papers/consistency-models.md) | 导读 | [一致性生成](concepts/consistency.md) · [条件生成](concepts/generation.md) |
| [Consistency Policy](papers/consistency-policy.md) | 导读 | [一致性生成](concepts/consistency.md) · [扩散去噪](concepts/diffusion.md) · [动作块](concepts/chunk.md) |
| [Cosmos Policy](papers/cosmos-policy.md) | 导读 | [世界动作联合建模](concepts/wam.md) · [视频时序生成](concepts/video.md) · [扩散去噪](concepts/diffusion.md) |
| [CoT-VLA](papers/cot-vla.md) | 导读 | [视频时序生成](concepts/video.md) · [动作表示](concepts/action.md) · [因果序列建模](concepts/causal.md) |
| [CQL](papers/cql.md) | 导读 | [离线强化学习](concepts/offline.md) · [价值估计与校准](concepts/value.md) · [策略与价值学习](concepts/actor-critic.md) |
| [Ctrl-World](papers/ctrl-world.md) | 导读 | [视频时序生成](concepts/video.md) · [动作条件动力学](concepts/dynamics.md) · [闭环滚动与历史偏移](concepts/rollout.md) |
| [DayDreamer](papers/daydreamer.md) | 导读 | [动作条件动力学](concepts/dynamics.md) · [想象轨迹训练](concepts/imagination.md) · [闭环滚动与历史偏移](concepts/rollout.md) |
| [DDIM](papers/ddim.md) | 导读 | [扩散去噪](concepts/diffusion.md) · [条件生成](concepts/generation.md) |
| [DDPM](papers/ddpm.md) | 导读 | [扩散去噪](concepts/diffusion.md) · [条件生成](concepts/generation.md) |
| [Decision Transformer](papers/decision-transformer.md) | 导读 | [因果序列建模](concepts/causal.md) · [动作表示](concepts/action.md) · [离线强化学习](concepts/offline.md) |
| [Deep WBC](papers/deep-whole-body-control.md) | 导读 | [全身控制与执行](concepts/wbc.md) · [环境适应](concepts/adaptation.md) · [强化学习](concepts/rl.md) |
| [DeepMimic](papers/deepmimic.md) | 导读 | [动作先验](concepts/motion-prior.md) · [强化学习](concepts/rl.md) · [全身控制与执行](concepts/wbc.md) |
| [Dex-One2Many](papers/dex-one2many.md) | 导读 | [空间表示](concepts/spatial.md) · [强化学习](concepts/rl.md) · [机器人数据与评测](concepts/data.md) |
| [DiffContact](papers/diffcontact.md) | 导读 | [动作条件动力学](concepts/dynamics.md) · [强化学习](concepts/rl.md) · [闭环滚动与历史偏移](concepts/rollout.md) · [PPO 与并行模拟](concepts/ppo.md) · [仿真到实机](concepts/sim2real.md) |
| [Diffuser](papers/diffuser.md) | 导读 | [扩散去噪](concepts/diffusion.md) · [树搜索与轨迹搜索](concepts/search.md) · [动作表示](concepts/action.md) |
| [Diffusion Forcing](papers/diffusion-forcing.md) | 导读 | [扩散去噪](concepts/diffusion.md) · [因果序列建模](concepts/causal.md) · [视频时序生成](concepts/video.md) |
| [Diffusion Policy](papers/diffusion-policy.md) | 导读 | [扩散去噪](concepts/diffusion.md) · [动作块](concepts/chunk.md) · [闭环滚动与历史偏移](concepts/rollout.md) |
| [DINO](papers/dino.md) | 导读 | [教师学生蒸馏](concepts/distill.md) · [交叉熵](concepts/cross-entropy.md) · [表征空间](concepts/representation.md) |
| [DINOv2](papers/dinov2.md) | 导读 | [教师学生蒸馏](concepts/distill.md) · [视觉 patch token](concepts/patches.md) · [表征空间](concepts/representation.md) |
| [DiT](papers/dit.md) | 导读 | [Diffusion Transformer](concepts/dit.md) · [视觉 patch token](concepts/patches.md) · [注意力](concepts/attention.md) |
| [DP3](papers/dp3.md) | 导读 | [点云与三维体素](concepts/point-cloud.md) · [扩散去噪](concepts/diffusion.md) · [动作块](concepts/chunk.md) |
| [Dreamer](papers/dreamer.md) | 导读 | [动作条件动力学](concepts/dynamics.md) · [想象轨迹训练](concepts/imagination.md) · [策略与价值学习](concepts/actor-critic.md) |
| [DreamerV2](papers/dreamerv2.md) | 导读 | [动作条件动力学](concepts/dynamics.md) · [想象轨迹训练](concepts/imagination.md) · [离散编码与量化](concepts/quantization.md) |
| [DreamerV3](papers/dreamerv3.md) | 导读 | [动作条件动力学](concepts/dynamics.md) · [想象轨迹训练](concepts/imagination.md) · [策略与价值学习](concepts/actor-critic.md) |
| [DreamTrue](papers/dreamtrue.md) | 导读 | [动作条件动力学](concepts/dynamics.md) · [视频时序生成](concepts/video.md) · [价值估计与校准](concepts/value.md) |
| [DreamWaQ](papers/dreamwaq.md) | 导读 | [特权训练信息](concepts/privileged.md) · [变分自编码器 VAE](concepts/vae.md) · [环境适应](concepts/adaptation.md) |
| [DreamZero](papers/dreamzero.md) | 导读 | [世界动作联合建模](concepts/wam.md) · [视频时序生成](concepts/video.md) · [动作表示](concepts/action.md) |
| [DROID](papers/droid.md) | 导读 | [机器人数据与评测](concepts/data.md) · [跨本体数据](concepts/cross-body.md) · [行为克隆](concepts/bc.md) |
| [EDM](papers/edm.md) | 导读 | [扩散去噪](concepts/diffusion.md) · [去噪网络预条件化](concepts/preconditioning.md) · [条件生成](concepts/generation.md) |
| [EfficientZero](papers/efficientzero.md) | 导读 | [动作条件动力学](concepts/dynamics.md) · [树搜索与轨迹搜索](concepts/search.md) · [表征空间](concepts/representation.md) |
| [EfficientZero V2](papers/efficientzero-v2.md) | 导读 | [动作条件动力学](concepts/dynamics.md) · [树搜索与轨迹搜索](concepts/search.md) · [价值估计与校准](concepts/value.md) |
| [EgoScale](papers/egoscale.md) | 导读 | [Flow Matching](concepts/flow.md) · [运动重定向](concepts/retarget.md) · [跨本体数据](concepts/cross-body.md) |
| [ExBody](papers/exbody.md) | 导读 | [运动重定向](concepts/retarget.md) · [全身控制与执行](concepts/wbc.md) · [动作先验](concepts/motion-prior.md) |
| [Extreme Parkour](papers/extreme-parkour.md) | 导读 | [特权训练信息](concepts/privileged.md) · [教师学生蒸馏](concepts/distill.md) · [仿真到实机](concepts/sim2real.md) |
| [FAST](papers/fast.md) | 导读 | [DCT 频率系数](concepts/dct.md) · [离散编码与量化](concepts/quantization.md) · [因果序列建模](concepts/causal.md) |
| [FLoRe](papers/flore.md) | 导读 | [示范模仿](concepts/imitation.md) · [扩散去噪](concepts/diffusion.md) · [动作块](concepts/chunk.md) · [全身控制与执行](concepts/wbc.md) · [仿真到实机](concepts/sim2real.md) · [运动重定向](concepts/retarget.md) · [动作表示](concepts/action.md) · [机器人数据与评测](concepts/data.md) |
| [Flow Matching](papers/flow-matching.md) | 导读 | [Flow Matching](concepts/flow.md) · [条件生成](concepts/generation.md) |
| [3DGS](papers/gaussian-splatting.md) | 导读 | [新视角场景表示](concepts/radiance.md) · [空间表示](concepts/spatial.md) · [表征空间](concepts/representation.md) |
| [GR00T N1](papers/gr00t-n1.md) | 导读 | [Flow Matching](concepts/flow.md) · [Diffusion Transformer](concepts/dit.md) · [跨本体数据](concepts/cross-body.md) |
| [Holo-M](papers/holo-m.md) | 已精讲 | [DCT 频率系数](concepts/dct.md) · [残差向量量化 RVQ](concepts/rvq.md) · [动作块](concepts/chunk.md) · [全身控制与执行](concepts/wbc.md) · [跨本体数据](concepts/cross-body.md) |
| [HOVER](papers/hover.md) | 导读 | [教师学生蒸馏](concepts/distill.md) · [遮蔽预测](concepts/masking.md) · [全身控制与执行](concepts/wbc.md) |
| [HumanPlus](papers/humanplus.md) | 导读 | [运动重定向](concepts/retarget.md) · [示范模仿](concepts/imitation.md) · [全身控制与执行](concepts/wbc.md) |
| [I-JEPA](papers/i-jepa.md) | 导读 | [表征预测 JEPA](concepts/jepa.md) · [遮蔽预测](concepts/masking.md) · [表征空间](concepts/representation.md) |
| [IQL](papers/iql.md) | 导读 | [离线强化学习](concepts/offline.md) · [价值估计与校准](concepts/value.md) · [行为克隆](concepts/bc.md) |
| [Isaac Gym](papers/isaac-gym.md) | 导读 | [PPO 与并行模拟](concepts/ppo.md) · [强化学习](concepts/rl.md) |
| [JAM](papers/jam.md) | 导读 | [表征空间](concepts/representation.md) · [表征预测 JEPA](concepts/jepa.md) · [余弦相似度](concepts/cosine.md) · [Flow Matching](concepts/flow.md) · [动作块](concepts/chunk.md) · [变分自编码器 VAE](concepts/vae.md) · [动作表示](concepts/action.md) · [分布偏移](concepts/shift.md) · [泛化评测与遗忘](concepts/benchmark.md) |
| [Latent Diffusion](papers/latent-diffusion.md) | 导读 | [扩散去噪](concepts/diffusion.md) · [注意力](concepts/attention.md) · [表征空间](concepts/representation.md) |
| [Dynamics Review](papers/learned-dynamics-review.md) | 导读 | [动作条件动力学](concepts/dynamics.md) · [空间表示](concepts/spatial.md) · [表征空间](concepts/representation.md) |
| [LeWAM](papers/lewam.md) | 导读 | [表征预测 JEPA](concepts/jepa.md) · [动作条件动力学](concepts/dynamics.md) · [逆动力学](concepts/inverse.md) · [模型预测控制 MPC](concepts/mpc.md) |
| [LeWM](papers/lewm.md) | 导读 | [表征预测 JEPA](concepts/jepa.md) · [动作条件动力学](concepts/dynamics.md) · [模型预测控制 MPC](concepts/mpc.md) |
| [LIBERO](papers/libero.md) | 导读 | [泛化评测与遗忘](concepts/benchmark.md) · [行为克隆](concepts/bc.md) · [机器人数据与评测](concepts/data.md) |
| [LingBot-VA](papers/lingbot-va.md) | 导读 | [世界动作联合建模](concepts/wam.md) · [变分自编码器 VAE](concepts/vae.md) · [因果序列建模](concepts/causal.md) · [闭环滚动与历史偏移](concepts/rollout.md) |
| [MAE](papers/mae.md) | 导读 | [遮蔽预测](concepts/masking.md) · [视觉 patch token](concepts/patches.md) · [表征空间](concepts/representation.md) |
| [MaskedMimic](papers/maskedmimic.md) | 导读 | [遮蔽预测](concepts/masking.md) · [教师学生蒸馏](concepts/distill.md) · [动作先验](concepts/motion-prior.md) |
| [MimicGen](papers/mimicgen.md) | 导读 | [机器人数据与评测](concepts/data.md) · [运动重定向](concepts/retarget.md) · [行为克隆](concepts/bc.md) |
| [Mobile ALOHA](papers/mobile-aloha.md) | 导读 | [行为克隆](concepts/bc.md) · [动作块](concepts/chunk.md) · [全身控制与执行](concepts/wbc.md) |
| [ModAR](papers/modar.md) | 导读 | [世界动作联合建模](concepts/wam.md) · [Diffusion Transformer](concepts/dit.md) · [因果序列建模](concepts/causal.md) |
| [MuZero](papers/muzero.md) | 导读 | [动作条件动力学](concepts/dynamics.md) · [树搜索与轨迹搜索](concepts/search.md) · [价值估计与校准](concepts/value.md) |
| [NeRF](papers/nerf.md) | 导读 | [新视角场景表示](concepts/radiance.md) · [空间表示](concepts/spatial.md) · [表征空间](concepts/representation.md) |
| [Octo](papers/octo.md) | 导读 | [扩散去噪](concepts/diffusion.md) · [动作块](concepts/chunk.md) · [跨本体数据](concepts/cross-body.md) |
| [OmniH2O](papers/omnih2o.md) | 导读 | [特权训练信息](concepts/privileged.md) · [教师学生蒸馏](concepts/distill.md) · [全身控制与执行](concepts/wbc.md) |
| [OpenVLA](papers/openvla.md) | 导读 | [离散编码与量化](concepts/quantization.md) · [跨本体数据](concepts/cross-body.md) · [表征空间](concepts/representation.md) |
| [PaLM-E](papers/palm-e.md) | 导读 | [表征空间](concepts/representation.md) · [因果序列建模](concepts/causal.md) · [分层技能与计划](concepts/skills.md) |
| [PerAct](papers/peract.md) | 导读 | [点云与三维体素](concepts/point-cloud.md) · [注意力](concepts/attention.md) · [空间表示](concepts/spatial.md) |
| [Perceptive Locomotion](papers/perceptive-loco.md) | 导读 | [空间表示](concepts/spatial.md) · [环境适应](concepts/adaptation.md) · [仿真到实机](concepts/sim2real.md) |
| [PHC](papers/phc.md) | 导读 | [动作先验](concepts/motion-prior.md) · [分层技能与计划](concepts/skills.md) · [全身控制与执行](concepts/wbc.md) |
| [Phenaki](papers/phenaki.md) | 导读 | [视频时序生成](concepts/video.md) · [离散编码与量化](concepts/quantization.md) · [遮蔽预测](concepts/masking.md) |
| [π₀](papers/pi0.md) | 导读 | [Flow Matching](concepts/flow.md) · [动作块](concepts/chunk.md) · [注意力](concepts/attention.md) |
| [π₀.₅](papers/pi05.md) | 导读 | [分层技能与计划](concepts/skills.md) · [跨本体数据](concepts/cross-body.md) · [Flow Matching](concepts/flow.md) |
| [PLaW-VLA](papers/plaw-vla.md) | 导读 | [表征预测 JEPA](concepts/jepa.md) · [因果序列建模](concepts/causal.md) · [动作表示](concepts/action.md) |
| [R3M](papers/r3m.md) | 导读 | [对比学习](concepts/contrastive.md) · [表征空间](concepts/representation.md) · [行为克隆](concepts/bc.md) |
| [Rectified Flow](papers/rectified-flow.md) | 导读 | [Flow Matching](concepts/flow.md) · [条件生成](concepts/generation.md) |
| [RMA](papers/rma.md) | 导读 | [特权训练信息](concepts/privileged.md) · [环境适应](concepts/adaptation.md) · [仿真到实机](concepts/sim2real.md) |
| [RoboCasa](papers/robocasa.md) | 导读 | [泛化评测与遗忘](concepts/benchmark.md) · [机器人数据与评测](concepts/data.md) · [行为克隆](concepts/bc.md) |
| [robomimic](papers/robomimic.md) | 导读 | [行为克隆](concepts/bc.md) · [离线强化学习](concepts/offline.md) · [机器人数据与评测](concepts/data.md) |
| [RT-1](papers/rt1.md) | 导读 | [注意力](concepts/attention.md) · [离散编码与量化](concepts/quantization.md) · [跨本体数据](concepts/cross-body.md) |
| [RT-2](papers/rt2.md) | 导读 | [离散编码与量化](concepts/quantization.md) · [跨本体数据](concepts/cross-body.md) · [因果序列建模](concepts/causal.md) |
| [Open X-Embodiment](papers/rtx.md) | 导读 | [跨本体数据](concepts/cross-body.md) · [机器人数据与评测](concepts/data.md) · [动作表示](concepts/action.md) |
| [RVT](papers/rvt.md) | 导读 | [空间表示](concepts/spatial.md) · [注意力](concepts/attention.md) · [点云与三维体素](concepts/point-cloud.md) |
| [RVT-2](papers/rvt2.md) | 导读 | [空间表示](concepts/spatial.md) · [注意力](concepts/attention.md) · [点云与三维体素](concepts/point-cloud.md) |
| [SAM](papers/sam.md) | 导读 | [空间表示](concepts/spatial.md) · [注意力](concepts/attention.md) · [零样本任务接口](concepts/zero-shot.md) |
| [SAM 2](papers/sam2.md) | 导读 | [空间表示](concepts/spatial.md) · [注意力](concepts/attention.md) · [闭环滚动与历史偏移](concepts/rollout.md) |
| [SayCan](papers/saycan.md) | 导读 | [分层技能与计划](concepts/skills.md) · [价值估计与校准](concepts/value.md) · [零样本任务接口](concepts/zero-shot.md) |
| [Self Forcing](papers/self-forcing.md) | 导读 | [视频时序生成](concepts/video.md) · [因果序列建模](concepts/causal.md) · [闭环滚动与历史偏移](concepts/rollout.md) |
| [SONIC](papers/sonic.md) | 导读 | [离散编码与量化](concepts/quantization.md) · [全身控制与执行](concepts/wbc.md) · [PPO 与并行模拟](concepts/ppo.md) |
| [SuperMimic](papers/supermimic.md) | 导读 | [世界模型](concepts/world.md) · [动作条件动力学](concepts/dynamics.md) · [想象轨迹训练](concepts/imagination.md) · [策略与价值学习](concepts/actor-critic.md) · [全身控制与执行](concepts/wbc.md) · [仿真到实机](concepts/sim2real.md) · [运动重定向](concepts/retarget.md) |
| [TD-MPC](papers/td-mpc.md) | 导读 | [动作条件动力学](concepts/dynamics.md) · [模型预测控制 MPC](concepts/mpc.md) · [价值估计与校准](concepts/value.md) |
| [TD-MPC2](papers/td-mpc2.md) | 导读 | [动作条件动力学](concepts/dynamics.md) · [模型预测控制 MPC](concepts/mpc.md) · [价值估计与校准](concepts/value.md) |
| [TD3+BC](papers/td3-bc.md) | 导读 | [离线强化学习](concepts/offline.md) · [策略与价值学习](concepts/actor-critic.md) · [行为克隆](concepts/bc.md) |
| [TOPS](papers/tops.md) | 导读 | [Flow Matching](concepts/flow.md) · [动作表示](concepts/action.md) · [动作块](concepts/chunk.md) · [示范模仿](concepts/imitation.md) · [泛化评测与遗忘](concepts/benchmark.md) · [分布偏移](concepts/shift.md) |
| [Trajectory Transformer](papers/trajectory-transformer.md) | 导读 | [因果序列建模](concepts/causal.md) · [离散编码与量化](concepts/quantization.md) · [树搜索与轨迹搜索](concepts/search.md) |
| [Transporter](papers/transporter.md) | 导读 | [空间表示](concepts/spatial.md) · [行为克隆](concepts/bc.md) · [动作表示](concepts/action.md) |
| [UMI](papers/umi.md) | 导读 | [运动重定向](concepts/retarget.md) · [动作表示](concepts/action.md) · [行为克隆](concepts/bc.md) |
| [UniPi](papers/unipi.md) | 导读 | [视频时序生成](concepts/video.md) · [逆动力学](concepts/inverse.md) · [扩散去噪](concepts/diffusion.md) |
| [VC-1](papers/vc1.md) | 导读 | [遮蔽预测](concepts/masking.md) · [视觉 patch token](concepts/patches.md) · [泛化评测与遗忘](concepts/benchmark.md) |
| [Video Diffusion](papers/video-diffusion.md) | 导读 | [视频时序生成](concepts/video.md) · [扩散去噪](concepts/diffusion.md) · [注意力](concepts/attention.md) |
| [VideoVLA](papers/videovla.md) | 导读 | [世界动作联合建模](concepts/wam.md) · [视频时序生成](concepts/video.md) · [动作表示](concepts/action.md) |
| [VIMA](papers/vima.md) | 导读 | [注意力](concepts/attention.md) · [因果序列建模](concepts/causal.md) · [泛化评测与遗忘](concepts/benchmark.md) |
| [VIOLA](papers/viola.md) | 导读 | [表征空间](concepts/representation.md) · [动作先验](concepts/motion-prior.md) · [跨本体数据](concepts/cross-body.md) |
| [VIP](papers/vip.md) | 导读 | [价值估计与校准](concepts/value.md) · [表征空间](concepts/representation.md) · [强化学习](concepts/rl.md) |
| [ViT](papers/vit.md) | 导读 | [视觉 patch token](concepts/patches.md) · [注意力](concepts/attention.md) · [表征空间](concepts/representation.md) |
| [V-JEPA 2](papers/vjepa2.md) | 导读 | [表征预测 JEPA](concepts/jepa.md) · [动作条件动力学](concepts/dynamics.md) · [模型预测控制 MPC](concepts/mpc.md) |
| [VQ-BeT](papers/vq-bet.md) | 导读 | [残差向量量化 RVQ](concepts/rvq.md) · [离散编码与量化](concepts/quantization.md) · [因果序列建模](concepts/causal.md) |
| [Legged Gym](papers/walk-in-minutes.md) | 导读 | [PPO 与并行模拟](concepts/ppo.md) · [仿真到实机](concepts/sim2real.md) · [环境适应](concepts/adaptation.md) |
| [Walk in the Park](papers/walk-in-the-park.md) | 导读 | [策略与价值学习](concepts/actor-critic.md) · [闭环滚动与历史偏移](concepts/rollout.md) · [动作表示](concepts/action.md) |
| [Walk These Ways](papers/walk-these-ways.md) | 导读 | [分层技能与计划](concepts/skills.md) · [动作表示](concepts/action.md) · [环境适应](concepts/adaptation.md) |

[具身榜](../leaderboard/README.md) · [论文地图](../paper-map/README.md) · [首页](../README.md)
