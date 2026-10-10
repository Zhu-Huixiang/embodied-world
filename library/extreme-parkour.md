# Extreme Parkour with Legged Robots

出处：ICRA 2024。研究范围：视觉四足跑酷与 sim-to-real。

[原文入口](https://ieeexplore.ieee.org/document/10610200) · [原文 PDF](https://extreme-parkour.github.io/resources/parkour.pdf) · [作者项目 / 代码入口](https://extreme-parkour.github.io/)

IEEE 向 Crossref 登记的题名与 DOI 对应 2024 IEEE International Conference on Robotics and Automation (ICRA)，published 日期 2024-05-13；IEEE Xplore document 10610200 对应同一题名。项目所列 CoRL 2023 是 Generalist/Roboletics/Deployable Workshop，不按 CoRL 主会归档。

阅读问题：**低频深度相机和不精确电机，怎样还能触发踩点精确的跳跃？**

收录理由：具身感知到控制耦合的清晰代表作，真实低成本四足跨跳、斜坡和手倒立，方法与直观视频都能支撑高质量选题。

证据入口：闭环视觉到关节控制、实机障碍课程和关键组件消融具备扎实证据；正式 ICRA 与公开项目支持追读。

具身关联：具身感知到控制耦合的清晰代表作，真实低成本四足跨跳、斜坡和手倒立，方法与直观视频都能支撑高质量选题。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/extreme-parkour/README.md)

机制简析：先在模拟中用特权地形训练策略，再把运动控制和行进方向一起蒸馏到深度图像学生。统一奖励让不同障碍上的动作自行形成，深度网络给策略提供地形潜变量与目标方向，本体策略输出关节命令。实机验证跨沟、上箱、斜坡等任务，并消融方向蒸馏与净空奖励。
<!-- discovery:end -->
