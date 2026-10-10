# Deep Whole-Body Control: Learning a Unified Policy for Manipulation and Locomotion

出处：CoRL 2022。研究范围：四足机械臂统一全身 RL。

[原文入口](https://proceedings.mlr.press/v205/fu23a.html) · [原文 PDF](https://proceedings.mlr.press/v205/fu23a/fu23a.pdf) · [作者项目 / 代码入口](https://manipulation-locomotion.github.io/)

CoRL 2022；PMLR 205 论文集出版年为 2023。

阅读问题：**手臂和腿一起出动作，怎样避免一边拿东西、一边把身体拽倒？**

收录理由：手脚协同的明确经典问题，统一策略、Advantage Mixing 与在线适应三个机制都有对照，是全身控制前置阅读。

证据入口：有统一与分离策略直接对照、关键训练机制消融和完整实机系统，能具体说明全身控制为什么需要协同。

具身关联：手脚协同的明确经典问题，统一策略、Advantage Mixing 与在线适应三个机制都有对照，是全身控制前置阅读。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/deep-whole-body-control/README.md)

机制简析：同一个网络接收底盘、腿、手臂状态和任务命令，输出六维手臂与十二维腿部关节目标，再由 PD 转为力矩。Advantage Mixing 把移动和操作的收益联系起来，Regularized Online Adaptation 对齐历史估计与训练环境信息。实验比较分开的控制器、未协调策略和适应方法，并在四足机械臂上验证。
<!-- discovery:end -->
