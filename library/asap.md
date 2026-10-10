# ASAP: Aligning Simulation and Real-World Physics for Learning Agile Humanoid Whole-Body Skills

出处：RSS 2025。研究范围：人形动作跟踪与数据驱动 sim-to-real。

[原文入口](https://www.roboticsproceedings.org/rss21/p066.html) · [原文 PDF](https://agile.human2humanoid.com/static/asap.pdf) · [作者项目 / 代码入口](https://agile.human2humanoid.com/)

RSS 2025；RSS PDF 的 Exa 正文为空，方法与实验初读改用作者正式 PDF。

阅读问题：**模拟和实机差一点，为什么补动作残差比盲目加大随机化更有针对性？**

收录理由：人形敏捷动作的明确动力学修正路线，RSS 正式论文与公开项目，具备高关注度选题所需的实机和方法细节。

证据入口：正式 RSS、两阶段数据链路明确，跨模拟器和实机与多种差距补偿基线比较；追读时能细讲残差学习而非只看动作视频。

具身关联：人形敏捷动作的明确动力学修正路线，RSS 正式论文与公开项目，具备高关注度选题所需的实机和方法细节。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/asap/README.md)

机制简析：先在模拟里训练人类动作跟踪策略，再在实机执行并记录轨迹。用真实轨迹训练 delta action 模型，找出能让模拟运动贴近真实运动的动作修正，把它接回模拟器后微调跟踪策略。原文比较跨模拟器和 Unitree G1 实机迁移，并对照系统辨识、域随机化与动力学残差。
<!-- discovery:end -->
