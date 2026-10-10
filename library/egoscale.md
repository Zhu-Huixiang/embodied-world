# EgoScale: Scaling Dexterous Manipulation with Diverse Egocentric Human Data

出处：arXiv 2026。研究范围：人类第一视角动作监督、灵巧手操作和跨本体迁移。

[原文入口](https://arxiv.org/abs/2602.16710) · [原文 PDF](https://arxiv.org/pdf/2602.16710v1) · [作者项目 / 代码入口](https://research.nvidia.com/labs/gear/egoscale/)

独立原研究2602.16710；仅核到预印本。one-shot仍有100条对齐human demos/对象与aligned midtraining，不能写成单条示范裸迁移。G1下肢由独立Homie策略执行，不把上肢VLA当全身端到端控制。

阅读问题：**人类视频怎样变成机器人可学的手腕和手指动作，为什么大量预训练之后还要一小段人机对齐数据？**

收录理由：用实机实验把human-video scaling与动作表示/本体对齐连接起来，且被N1.7实际采用；机制和代价足够清楚，适合研究性解读而非发布新闻。

证据入口：20854小时human wrist+retargeted hand-action supervision；flow-based VLA+DiT；aligned human–robot midtraining；22DoFSharpa手，腕部相对SE(3)，低DoF本体adapter。（§2.1–2.5/Fig1–2）；5项高灵巧实机任务，常规100robot demos/task，shirt rolling20；比较scratch、midtrain-only、human-pretrain、human-pretrain+midtrain，分别报告completion score和binary success。两seed；常规每seed10trials，bottle4实例各4trials（原文TaskIII标签与bottle描述有错配，正式精读需核图表/附录）。（§3.1–3.2/Fig3–4）；1k/2k/4k/10k/20k小时pretrain规模；平均task completion由0.30到0.71。human validation 2000episodes×20timesteps，每时刻16sample平均action；L=0.024−0.003ln(D)，R²0.9983是在测量范围内的五档拟合。（§3.3/Fig5/Eq1）

具身关联：人类第一视角动作监督、灵巧手操作和跨本体迁移；人类视频怎样变成机器人可学的手腕和手指动作，为什么大量预训练之后还要一小段人机对齐数据？

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/egoscale/README.md)

机制简析：从第一视角human videos提取相对SE(3)腕部轨迹与重定向22DoF手关节，pretrain flow-based VLA；少量paired human/robot play midtraining对齐视觉和motor接口，再任务posttrain。统一腕部action、embodiment-specific hand/state adapters迁移至G1 7DoF手，下肢独立Homie。
<!-- discovery:end -->
