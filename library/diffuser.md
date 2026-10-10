# Planning with Diffusion for Flexible Behavior Synthesis

出处：ICML 2022。研究范围：扩散轨迹规划基础；模拟控制。

[原文入口](https://proceedings.mlr.press/v162/janner22a.html) · [原文 PDF](https://proceedings.mlr.press/v162/janner22a/janner22a.pdf) · [作者项目 / 代码入口](https://diffusion-planning.github.io/)

阅读问题：**轨迹一起去噪，如何同时承担环境建模、长时序规划与测试时加约束？**

收录理由：扩散生成接到控制规划的基础论文，区别于只生成一步动作，适合解释后续扩散策略和世界动作模型的来路。

证据入口：提出可组合的生成式规划框架，有长时序控制及条件变化实验，正式 ICML 论文和官方项目可复核。

具身关联：扩散生成接到控制规划的基础论文，区别于只生成一步动作，适合解释后续扩散策略和世界动作模型的来路。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/diffuser/README.md)

机制简析：Diffuser 学习整段状态—动作轨迹的去噪过程，反复修正所有规划时刻，而不是单步滚动一个动力学模型。奖励梯度可以引导去噪，固定起点或终点则像图像补全那样锁住轨迹部分。论文在长时序与灵活测试条件下比较规划效果，并区分扩散步和环境时间步。
<!-- discovery:end -->
