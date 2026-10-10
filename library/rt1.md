# RT-1: Robotics Transformer for Real-World Control at Scale

出处：RSS 2023。研究范围：语言条件的多任务真实机器人操作与移动控制。

[原文入口](https://www.roboticsproceedings.org/rss19/p025.html) · [原文 PDF](https://roboticsproceedings.org/rss19/p025.pdf) · [作者项目 / 代码入口](https://robotics-transformer1.github.io/)

以 RSS 2023 正式论文为收录版，RT-1 与 RT-2 分条；不是把语言模型直接当低层控制器。

阅读问题：**大量真实机器人数据究竟需要什么策略结构才能吃进去，TokenLearner 为何是关键？**

收录理由：机器人 Transformer 规模化控制路线的早期核心工作，后续 RT-2、RT-X 与通用机器人策略讨论的直接基础；有大规模真实数据、模型与数据消融。

证据入口：RSS 正式 PDF 与项目页给出 BC-Z、Gato 对照、数据量/数据多样性消融和真实厨房评估，证据丰富；开源模型和数据提供复用入口。

具身关联：机器人 Transformer 规模化控制路线的早期核心工作，后续 RT-2、RT-X 与通用机器人策略讨论的直接基础；有大规模真实数据、模型与数据消融。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/rt1/README.md)

机制简析：图像先经语言条件的 EfficientNet 提取特征，再由 TokenLearner 压成少量视觉 token；Transformer 融合短时历史并输出离散动作。动作同时覆盖机械臂、底盘和停止模式，策略以闭环方式反复读取图像。原文分别检验新指令、干扰物、新背景以及跨机器人数据混合的效果。
<!-- discovery:end -->
