# BridgeData V2: A Dataset for Robot Learning at Scale

出处：CoRL 2023。研究范围：多环境真实操作数据、语言/目标条件策略与泛化。

[原文入口](https://proceedings.mlr.press/v229/walke23a.html) · [原文 PDF](https://proceedings.mlr.press/v229/walke23a/walke23a.pdf) · [作者项目 / 代码入口](https://rail-berkeley.github.io/bridgedata/)

PMLR HTML 摘要记 53,896 轨迹，正式 PDF/当前项目页记 60,096；精读固定版并逐项核对，不混抄数据总量。

阅读问题：**机器人数据怎样覆盖场景差异，才会支持跨环境与跨机构技能迁移？**

收录理由：广泛复用的真实机器人操作数据节点，连接跨环境预训练、Open X-Embodiment 和开放通用策略。

证据入口：CoRL 正式版与项目提供多环境数据、多个离线算法及数据/容量研究，开放数据、预训练模型和硬件指南复用价值很高；贡献主要在可泛化数据基础设施。

具身关联：广泛复用的真实机器人操作数据节点，连接跨环境预训练、Open X-Embodiment 和开放通用策略。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/bridge-v2/README.md)

机制简析：统一低成本机械臂平台收集语言标注轨迹，同时主动变化物体、相机、场景和工作台位置。策略可按目标图或自然语言训练，测试再拆开已见任务的视觉变化与新物体、新环境泛化。不同离线学习方法、数据规模和模型容量在同一数据上比较，让数据多样性的作用有可检查的落点。
<!-- discovery:end -->
