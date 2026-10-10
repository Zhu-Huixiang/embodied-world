# Open X-Embodiment: Robotic Learning Datasets and RT-X Models

出处：ICRA 2024。研究范围：跨机器人数据标准化、RT-1-X/RT-2-X 通用操作策略。

[原文入口](https://ieeexplore.ieee.org/document/10611477) · [原文 PDF](https://arxiv.org/pdf/2310.08864) · [作者项目 / 代码入口](https://robotics-transformer-x.github.io/)

ICRA 2024 正式发表；PDF 入口为作者 arXiv 版本，精读需固定版本，勿合并项目后续新增数据统计。

阅读问题：**不同机器人的动作坐标和观测并不一致，怎样把它们混成能产生正迁移的数据？**

收录理由：跨机构、跨机器人联合训练的关键公共基础设施；ICRA 官方奖项页列为 Best Conference Paper Award 获奖工作。

证据入口：IEEE 正式入口确认 ICRA，官方奖项页确认获奖，原项目给出多平台正迁移及 RT-2-X 新技能测试；标准化数据和开放代码具有直接复用价值。

具身关联：跨机构、跨机器人联合训练的关键公共基础设施；ICRA 官方奖项页列为 Best Conference Paper Award 获奖工作。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/rtx/README.md)

机制简析：先把各实验室的轨迹变成统一数据格式，并以夹爪参考系中的位置、姿态和夹爪开合统一动作接口；未使用的动作分量按数据约定处理。RT-1-X 和 RT-2-X 在这个混合数据上训练，再与各机器人自己的专用数据策略比较。它检验的不是同一机器人多收点数据，而是别的机器人经验能否改善当前机器人。
<!-- discovery:end -->
