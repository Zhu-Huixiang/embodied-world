# Expressive Whole-Body Control for Humanoid Robots

**解读导读** · RSS 2024 · [Locomotion 与运动适应](../paper-map/README.md#track-locomotion)

研究范围：人形表达动作与稳健行走。

[原文入口](https://www.roboticsproceedings.org/rss20/p107.html) · [原文 PDF](https://www.roboticsproceedings.org/rss20/p107.pdf) · [作者项目 / 代码入口](https://expressive-humanoid.github.io/) · [作者与团队](../leaderboard/origins/papers/exbody.md)

RSS 2024 正式主会。

## 先看它做了什么

从人类动作库筛选并重定向姿态，训练时要求机器人上半身跟随关节和关键点目标。下半身放松逐关节模仿约束，改为跟随根速度和姿态命令，以留出平衡和行走空间。原文对照完整身体跟踪、分开策略与初始化方式，实机展示行走和表达动作。

## 带着什么问题读

**上半身想照着人动，下半身还得站稳，这两种目标怎么兼容？**

## 为什么值得继续读

在人形形态差异下提出可解释的约束取舍：上身跟踪、下身速度控制；是后续更完整全身跟踪路线的重要比较对象。

证据入口：正式 RSS，核心约束改动与完整跟踪基线直接比较，sim-to-real 与实机动作支持其科学问题。

具身关联：在人形形态差异下提出可解释的约束取舍：上身跟踪、下身速度控制；是后续更完整全身跟踪路线的重要比较对象。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/exbody/README.md) · [RSS集锦](../venues/RSS/README.md) · [地图方向](../paper-map/README.md#track-locomotion) · [首页](../README.md)

元数据核对：2026-10-10。
