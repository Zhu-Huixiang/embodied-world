# R3M: A Universal Visual Representation for Robot Manipulation

**解读导读** · CoRL 2022 · [具身感知与场景表示](../paper-map/README.md#track-embodied-perception)

研究范围：人类视频预训练视觉表征与少样本机器人学习。

[原文入口](https://proceedings.mlr.press/v205/nair23a.html) · [原文 PDF](https://proceedings.mlr.press/v205/nair23a/nair23a.pdf) · [作者项目 / 代码入口](https://sites.google.com/view/robot-r3m/home) · [作者与团队](../leaderboard/origins/papers/r3m.md)

CoRL 2022；PMLR 2023。R3M 是冻结视觉表示，不是直接生成机器人动作的 VLA。

## 先看它做了什么

在人类视频上联合时间对比、视频语言对齐和稀疏约束，让编码器同时记住场景变化与任务语义。下游冻结编码器，把图像向量交给机器人策略，只用少量机器人示范学习动作。原文比较从零训练、CLIP、MoCo 等视觉初始化，并在真实公寓中测试操作。

## 带着什么问题读

**人类第一视角视频里学来的视觉表征，怎样成为机器人少样本操作的感知模块？**

## 为什么值得继续读

人类视频到机器人表征迁移的代表基线，连接视频预训练、可迁移感知和少样本行为克隆。

证据入口：CoRL 正式版提供三种目标、多个仿真任务和真实少示范对照，公开预训练模型；后续 VC-1 系统研究把 R3M 列为核心对照。

具身关联：人类视频到机器人表征迁移的代表基线，连接视频预训练、可迁移感知和少样本行为克隆。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/r3m/README.md) · [CoRL集锦](../venues/CoRL/README.md) · [地图方向](../paper-map/README.md#track-embodied-perception) · [首页](../README.md)

元数据核对：2026-10-10。
