# SONIC: Supersizing Motion Tracking for Natural Humanoid Whole-Body Control

出处：Science-Robotics 2026。研究范围：大规模人形动作跟踪、全身低层控制、规划与VLA接口。

[原文入口](https://www.science.org/doi/10.1126/scirobotics.aed4592) · [原文 PDF](https://arxiv.org/pdf/2511.07820v4) · [作者项目 / 代码入口](https://nvlabs.github.io/GEAR-SONIC/)

正式刊文2026-08-12；本文数据按 arXiv v4 对应版本定位。比较跟踪基线时训练数据和重定向管线不同，五项VLA任务只有每项10–20次实机试验。避免把模型版本 SONIC v1.1 当第二篇论文。

阅读问题：**动作跟踪为什么能吃进大规模人类动作数据，64维共享运动 token 又怎样让同一控制器接遥操作和全身 VLA？**

收录理由：有正式刊文、三轴规模消融和全身实机执行，连接动作先验学习与VLA动作空间，是当前榜单的人形系统控制漏项。

证据入口：三类命令encoder→FSQ token→control decoder(token+10步本体历史)→joint-position targets→PD；auxiliary motion decoder重建；训练loss由PPO/recon/token/cycle组成。G1有29 actuated joints；控制50Hz，命令流500Hz；Jetson Orin forward1–2ms。（§3.2, Fig.6, Eq.(1)–(4); §3.5）；数据4M/10M/22M/100M帧、网络1.2M/16M/42M参数、算力约2k/9k/21k GPU小时三轴比较；最大网络test-content 99.6%及23.8mm MPJPE-L，最小网络98.0%及27.7mm。阴影为6次评测的均值±1sd。（§2.1 Scaling Up Motion Tracking / Fig.2(A–C)）；统一MuJoCo终止条件下，SONIC在test-content/test-repetition/PHUMA为98.5/99.2/97.2%，BeyondMimic82.0/85.4/73.8%；SONIC与基线训练数据/重定向不同，只能解释为此系统与数据组合的跨分布能力。（§2.1 Comparison with Other Motion Trackers）

具身关联：大规模人形动作跟踪、全身低层控制、规划与VLA接口；动作跟踪为什么能吃进大规模人类动作数据，64维共享运动 token 又怎样让同一控制器接遥操作和全身 VLA？

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/sonic/README.md)

机制简析：机器人/人体/稀疏混合命令分别编码到 FSQ 共享运动 token；同一控制解码器结合10步本体历史输出29关节目标，由PD执行。PPO与运动重建、token对齐和cycle损失联合训练；上游实时运动规划或VLA预测64维token与14维手关节。
<!-- discovery:end -->
