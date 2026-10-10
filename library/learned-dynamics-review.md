# A review of learning-based dynamics models for robotic manipulation

**解读导读** · Sci. Robot. 2025 · [世界模型与模型强化学习](../paper-map/README.md#track-world-model)

研究范围：机器人操作；学习动力学综述。

[原文入口](https://www.science.org/doi/10.1126/scirobotics.adt1497) · [原文 PDF](https://albertboai.com/assets/pdf/2025_scirobotics.adt1497.pdf) · [作者项目 / 代码入口](https://albertboai.com/)

Science Robotics 10(106), eadt1497；综述分按组织框架与证据综合，不冒充新算法实机结果。

## 先看它做了什么

以 POMDP/控制目标为入口，按像素、latent、粒子、关键点、物体中心表示比较动力学；再讨论感知和控制接口。

## 带着什么问题读

**世界模型该预测像素、latent、粒子还是物体？换种表示会怎样改写感知与规划的代价？**

## 为什么值得继续读

Science Robotics 正式综述；用表示选择贯通感知、动作条件动力学和控制，分类与证据综合有用，原创算法分不过度拔高。

证据入口：五种表示连接动力学、感知和控制；讨论 latent 重建式/无需重建目标与可变形、多物体任务。（Eq.1、Fig.2 与表示分类各节）

具身关联：机器人操作；学习动力学综述；世界模型该预测像素、latent、粒子还是物体？换种表示会怎样改写感知与规划的代价？

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/learned-dynamics-review/README.md) · [Sci. Robot.集锦](../venues/Science-Robotics/README.md) · [地图方向](../paper-map/README.md#track-world-model) · [首页](../README.md)

元数据核对：2026-10-10。
