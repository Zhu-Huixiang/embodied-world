# Perceiver-Actor: A Multi-Task Transformer for Robotic Manipulation

出处：CoRL 2022。研究范围：语言条件 6-DoF 操作、体素表示与 Perceiver。

[原文入口](https://proceedings.mlr.press/v205/shridhar23a.html) · [原文 PDF](https://proceedings.mlr.press/v205/shridhar23a/shridhar23a.pdf) · [作者项目 / 代码入口](https://peract.github.io/)

CoRL 2022；PMLR 书目年份 2023。

阅读问题：**把动作当成体素中的检测目标，为什么比从整张图片直接回归动作更省示范？**

收录理由：3D 动作检测式操作策略的代表作，后续 RVT/RVT-2 的直接对照基础。

证据入口：PMLR 正式 PDF 与项目给出完整体素/动作接口、RLBench 和真实平台对照，并有单 GPU 教程；计算成本也形成后续 RVT 的明确研究问题。

具身关联：3D 动作检测式操作策略的代表作，后续 RVT/RVT-2 的直接对照基础。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/peract/README.md)

机制简析：RGB-D 重建为三维体素网格，体素 patch 与语言向量组成序列；Perceiver 用少量 latent 承接长输入。输出逐体素特征后检测下一关键动作的位置，并预测离散旋转、夹爪及碰撞选项，交由运动规划器执行。网格把观测位置和动作位置对齐，原文再比较图像回归、3D 卷积与多任务少示范性能。
<!-- discovery:end -->
