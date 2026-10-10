# OmniH2O: Universal and Dexterous Human-to-Humanoid Whole-Body Teleoperation and Learning

出处：CoRL 2024。研究范围：人形全身遥操作、控制与自主模仿。

[原文入口](https://proceedings.mlr.press/v270/he25b.html) · [原文 PDF](https://raw.githubusercontent.com/mlresearch/v270/main/assets/he25b/he25b.pdf) · [作者项目 / 代码入口](https://omni.human2humanoid.com/)

CoRL 2024；PMLR 270 论文集出版年为 2025。

阅读问题：**只有头和双手目标，为什么还能指挥整个身体并收集自主学习数据？**

收录理由：统一姿态接口和教师学生迁移的代表工作，后续 ASAP 与 HOVER 路线直接相关；有姿态/历史/DAgger 消融及实机学习。

证据入口：有大规模跟踪、实机指标与 DAgger/历史/目标点消融，统一接口和公开数据支持后续复用。

具身关联：统一姿态接口和教师学生迁移的代表工作，后续 ASAP 与 HOVER 路线直接相关；有姿态/历史/DAgger 消融及实机学习。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/omnih2o/README.md)

机制简析：把不同遥操作方式转换成运动学姿态目标，再交给跟踪控制器。特权教师在模拟中学大规模动作，学生用本体历史与稀疏目标通过 DAgger 模仿教师，输出可部署的动作；手部另接姿态到关节控制。原文验证模拟和实机跟踪、不同控制入口及采集示范后的自主技能。
<!-- discovery:end -->
