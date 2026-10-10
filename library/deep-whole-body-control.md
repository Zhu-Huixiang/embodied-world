# Deep Whole-Body Control: Learning a Unified Policy for Manipulation and Locomotion

**解读导读** · CoRL 2022 · [Locomotion 与运动适应](../paper-map/README.md#track-locomotion)

研究范围：四足机械臂统一全身 RL。

[原文入口](https://proceedings.mlr.press/v205/fu23a.html) · [原文 PDF](https://proceedings.mlr.press/v205/fu23a/fu23a.pdf) · [作者项目 / 代码入口](https://manipulation-locomotion.github.io/) · [作者与团队](../leaderboard/origins/papers/deep-whole-body-control.md)

CoRL 2022；PMLR 205 论文集出版年为 2023。

## 先看它做了什么

同一个网络接收底盘、腿、手臂状态和任务命令，输出六维手臂与十二维腿部关节目标，再由 PD 转为力矩。Advantage Mixing 把移动和操作的收益联系起来，Regularized Online Adaptation 对齐历史估计与训练环境信息。实验比较分开的控制器、未协调策略和适应方法，并在四足机械臂上验证。

## 带着什么问题读

**手臂和腿一起出动作，怎样避免一边拿东西、一边把身体拽倒？**

## 为什么值得继续读

手脚协同的明确经典问题，统一策略、Advantage Mixing 与在线适应三个机制都有对照，是全身控制前置阅读。

证据入口：有统一与分离策略直接对照、关键训练机制消融和完整实机系统，能具体说明全身控制为什么需要协同。

具身关联：手脚协同的明确经典问题，统一策略、Advantage Mixing 与在线适应三个机制都有对照，是全身控制前置阅读。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/deep-whole-body-control/README.md) · [CoRL集锦](../venues/CoRL/README.md) · [地图方向](../paper-map/README.md#track-locomotion) · [首页](../README.md)

元数据核对：2026-10-10。
