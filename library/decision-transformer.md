# Decision Transformer: Reinforcement Learning via Sequence Modeling

出处：NeurIPS 2021。研究范围：序列决策基础；离线控制。

[原文入口](https://proceedings.neurips.cc/paper_files/paper/2021/hash/7f489f642a0ddb10272b5c31057f0663-Abstract.html) · [原文 PDF](https://proceedings.neurips.cc/paper_files/paper/2021/file/7f489f642a0ddb10272b5c31057f0663-Paper.pdf)

阅读问题：**把目标回报放进 token 序列，就能把离线控制改写成条件生成吗？**

收录理由：把决策问题接到 Transformer 的代表性路线；Trajectory Transformer 原文与它比较规划和回报条件化，适合进入动作语言模型的前置阅读。

证据入口：方法提出清晰的新决策表述，正式论文跨离散与连续域，后续 Trajectory Transformer 对其优缺点作直接比较。

具身关联：把决策问题接到 Transformer 的代表性路线；Trajectory Transformer 原文与它比较规划和回报条件化，适合进入动作语言模型的前置阅读。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/decision-transformer/README.md)

机制简析：把未来目标回报、状态和动作按时间交错成序列，因果 Transformer 用过去上下文预测当前动作。训练直接拟合数据动作；执行后减去已经获得的奖励，再把更新后的目标回报与新状态送回模型。实验用 Atari、Gym 与长时序任务检验这个条件生成式策略。
<!-- discovery:end -->
