# DayDreamer: World Models for Physical Robot Learning

出处：CoRL 2022。研究范围：真实机器人世界模型；行走、操作与导航。

[原文入口](https://proceedings.mlr.press/v205/wu23c.html) · [原文 PDF](https://proceedings.mlr.press/v205/wu23c/wu23c.pdf) · [作者项目 / 代码入口](https://danijar.com/project/daydreamer/)

CoRL 2022；PMLR 205 论文集出版年为 2023。

阅读问题：**世界模型的想象训练怎样接到真实机器人持续在线交互上？**

收录理由：把 Dreamer 从模拟基准接到四种实机平台，跨行走、视觉操作、导航，直接对应具身世界模型的落地问题。

证据入口：有多平台实机闭环与明确训练时间、学习曲线和基线；公开基础设施，使世界模型精讲能落到真实采样链路。

具身关联：把 Dreamer 从模拟基准接到四种实机平台，跨行走、视觉操作、导航，直接对应具身世界模型的落地问题。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/daydreamer/README.md)

机制简析：真实机器人持续把轨迹写入经验回放，学习线程更新潜空间世界模型，再用模型想象的轨迹训练策略和值函数。异步 actor 与 learner 把快速执行和较慢训练拆开，避免每次梯度更新卡住机器人控制。原文用四足、两种机械臂和轮式机器人检查同一算法的在线学习能力。
<!-- discovery:end -->
