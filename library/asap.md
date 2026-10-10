# ASAP: Aligning Simulation and Real-World Physics for Learning Agile Humanoid Whole-Body Skills

**解读导读** · RSS 2025 · [Locomotion 与运动适应](../paper-map/README.md#track-locomotion)

研究范围：人形动作跟踪与数据驱动 sim-to-real。

[原文入口](https://www.roboticsproceedings.org/rss21/p066.html) · [原文 PDF](https://agile.human2humanoid.com/static/asap.pdf) · [作者项目 / 代码入口](https://agile.human2humanoid.com/) · [作者与团队](../leaderboard/origins/papers/asap.md)

RSS 2025；RSS PDF 的 Exa 正文为空，方法与实验初读改用作者正式 PDF。

## 先看它做了什么

先在模拟里训练人类动作跟踪策略，再在实机执行并记录轨迹。用真实轨迹训练 delta action 模型，找出能让模拟运动贴近真实运动的动作修正，把它接回模拟器后微调跟踪策略。原文比较跨模拟器和 Unitree G1 实机迁移，并对照系统辨识、域随机化与动力学残差。

## 带着什么问题读

**模拟和实机差一点，为什么补动作残差比盲目加大随机化更有针对性？**

## 为什么值得继续读

人形敏捷动作的明确动力学修正路线，RSS 正式论文与公开项目，具备高关注度选题所需的实机和方法细节。

证据入口：正式 RSS、两阶段数据链路明确，跨模拟器和实机与多种差距补偿基线比较；追读时能细讲残差学习而非只看动作视频。

具身关联：人形敏捷动作的明确动力学修正路线，RSS 正式论文与公开项目，具备高关注度选题所需的实机和方法细节。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/asap/README.md) · [RSS集锦](../venues/RSS/README.md) · [地图方向](../paper-map/README.md#track-locomotion) · [首页](../README.md)

元数据核对：2026-10-10。
