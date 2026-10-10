# 补查与收录决定｜2026-10-10

本次补查围绕世界模型、WAM、人形控制和影响证据，累计250条Exa检索结果，逐篇再读官方出处、原文方法/实验和项目。这是检索结果计数，不是250篇全文精读。

新增10篇独立论文：5篇正式刊会、5篇精选预印本。LingBot-VA、π₀.₅、Cosmos Policy沿用已有条目并更新正式出处。全库115篇，每篇七维完整评分；正式精讲继续按总榜中已正式发表的论文排序。

## 正式刊会补充

| 论文 | 出处 | 收录依据 |
| --- | --- | --- |
| [SONIC](papers/sonic/README.md) | [Science Robotics 2026](https://www.science.org/doi/10.1126/scirobotics.aed4592) | 正式 Science Robotics 原研究；将大规模动作跟踪、共享控制 token、实时规划和 VLA 全身执行接成可用系统，具有数据/容量/算力三轴消融及模拟与实机证据。人形低层控制和 VLA 接口都直接相关，值得补入。分数仍保留对训练数据不对齐、有限实机试次与长期安全验证的扣分。 |
| [Ctrl-World](papers/ctrl-world/README.md) | [ICLR 2026](https://proceedings.iclr.cc/paper_files/paper/2026/hash/0ae94013da7cd459402fd77874e09ee3-Abstract-Conference.html) | 正式ICLR2026工作；多视角、逐帧动作条件、姿态条件记忆三个关键模块有单项消融，且做真实策略排名和合成数据回训。它直接把世界模型接入VLA评价与改进闭环，值得上榜，必须把指令遵循与低层物理成功区分。 |
| [Dynamics Review](papers/learned-dynamics-review/README.md) | [Science Robotics 2025](https://www.science.org/doi/10.1126/scirobotics.adt1497) | Science Robotics 正式综述；用表示选择贯通感知、动作条件动力学和控制，分类与证据综合有用，原创算法分不过度拔高。 |
| [HOVER](papers/hover/README.md) | [ICRA 2025](https://hover-versatile-humanoid.github.io/) | ICRA 2025 正式论文；oracle、命令 mask 和 DAgger 蒸馏有明确接口，仿真多模式对照与实机控制值得精选。 |
| [Isaac Gym](papers/isaac-gym/README.md) | [NeurIPS 2021 Datasets & Benchmarks](https://datasets-benchmarks-proceedings.neurips.cc/paper/2021/hash/28dd2c7955ce926456240b2ff0100bde-Abstract-round2.html) | 正式 NeurIPS 2021 D&B track；GPU 全链路物理与训练是腿足、人形、灵巧 RL 的基础设施漏收项。 |

## 精选预印本观察

正式发表轴记0；创新、实验与证据、影响和复用按实际材料评分。它们进入总榜，正式刊会精讲队列以后随身份更新。

| 论文 | 具体贡献与判断 |
| --- | --- |
| [LeWM](papers/lewm/README.md) | 与现有LeWAM是两篇不同工作。SIGReg将端到端像素JEPA防坍缩变成两项损失，在四环境、同计算预算和正则/编码器消融上给出可核对证据，官方公开训练代码、数据、模型和基线checkpoint，值得作为潜世界模型基础新作收录。正式刊会未核到，不进入正式刊会队列。 |
| [ModAR](papers/modar/README.md) | 新预印本有较强问题控制：统一backbone/训练预算比较多种WAM组织方式、独立IDM与相等采样步数，6任务仿真与3任务双臂实机。结构化未来先于动作的主张可检验，作为近期WAM候选值得上榜；不把75%vs72%的系统级对照写成全领域胜负。 |
| [GR00T N1](papers/gr00t-n1/README.md) | N1.7的可追溯原研究，现有目录缺少。真实方法/实验、开源模型和跨本体数据工程完整，且被正式LingBot-VA作为基线复用。保留原论文身份，按预印本入观察，不把官方research页的Type Conference paper字段误读成正式录用。 |
| [EgoScale](papers/egoscale/README.md) | 与N1.7关联的独立原研究，不是将版本发布当论文。大规模人类手腕/手指动作标注、数据规模研究、对齐midtraining和跨手型transfer均有实机证据，值得放入高价值预印本观察。正式venue查到的官方原入口仍arXiv，不自行猜CoRL/NeurIPS。 |
| [V-JEPA 2](papers/vjepa2/README.md) | 视频表征直接接动作条件预测与真实机器人 MPC；实验基线、条件和开放实现可读，按精选预印本收录。 |

## 已有条目更新

| 论文 | 本次核实 | 入口 |
| --- | --- | --- |
| [LingBot-VA](papers/lingbot-va/README.md) | RSS 2026 | [原始记录](https://www.roboticsproceedings.org/rss22/p016.html) |
| [π₀.₅](papers/pi05/README.md) | CoRL 2025 | [原始记录](https://proceedings.mlr.press/v305/black25a.html) |
| [Cosmos Policy](papers/cosmos-policy/README.md) | ICLR 2026 Poster | [原始记录](https://openreview.net/forum?id=wPEIStHxYH) |
| [DreamerV3](papers/dreamerv3/README.md) | Nature 2025；已有条目不重复 | [原始记录](https://www.nature.com/articles/s41586-025-08744-2) |
| [DreamZero](papers/dreamzero/README.md) | 维持预印本；当前官方虚拟页不能定位主会轨道 | [原始记录](https://arxiv.org/abs/2602.15922) |

## 这次暂缓/不另建

### DreamMimic

官方IROS2026身份成立，方法和消融值得读，可保留候选；当前高影响榜补充门槛暂缓：量化在SMPL-X仿真，depth/seg为仿真真值，G1/跨模拟器仅定性，代码未开且无已核独立采用信号；PCG与调好的naive annealing成功率相同，主要改善跟踪误差。不是判定水论文，也不因提名强塞为高影响工作。

[官方/原文依据1](https://2026.ieee-iros.org/program/paper-index/) · [官方/原文依据2](https://arxiv.org/abs/2608.22278) · [官方/原文依据3](https://arxiv.org/pdf/2608.22278v1) · [官方/原文依据4](https://dreammimic.github.io/)

### GR00T N1.7

拒绝作为独立论文上榜，而不是否定模型。官方于2026-04-17发布 N1.7 Early Access 模型和权重；模型卡把架构说明指回 GR00T N1 白皮书，发布说明把核心人类视频预训练研究指向 EgoScale。核到真实模型但没有独立 N1.7 论文身份，不能将产品/模型版号重复计为论文。

[官方/原文依据1](https://huggingface.co/nvidia/GR00T-N1.7-3B) · [官方/原文依据2](https://huggingface.co/blog/nvidia/gr00t-n1-7) · [官方/原文依据3](https://developer.nvidia.com/blog/develop-humanoid-robot-policies-end-to-end-with-nvidia-isaac-gr00t/) · [官方/原文依据4](https://github.com/NVIDIA/Isaac-GR00T)

## 版本与数据提醒

- LeWM和LeWAM是两篇不同研究。LeWM当前科学摘录读v1，最新已发现v3；正式精讲前复核新版本。
- SONIC采用对应正式刊文的v4；训练数据、baseline与VLA小样本试验按各自条件解释。
- LingBot-VA正式RSS Table I为92.0/91.1，不能混用arXiv v2的92.93/91.55；正式消融表另按原表条件。
- Ctrl-World的38.7%→83.4%是44.7个百分点。EgoScale one-shot还包括每对象100条aligned human demos及midtraining。
- 动力学综述按分类框架与证据综合评分，引用到的实机结果不当作综述自己的实验。
- 原始引用缺项保持null，所有上榜论文的影响/近期轴采用匹配引用公式或有来源的独立证据分；不把模型发布、作者机构或共用repo star当单篇影响。

[全部具身榜](README.md) · [评分规则](methodology.md) · [正式精讲队列](../calendar/queue.md)
