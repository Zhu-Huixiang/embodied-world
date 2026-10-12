# 本篇方法链路 · Decision Transformer

把未来目标回报、状态和动作按时间交错成序列，因果 Transformer 用过去上下文预测当前动作。训练直接拟合数据动作；执行后减去已经获得的奖励，再把更新后的目标回报与新状态送回模型。实验用 Atari、Gym 与长时序任务检验这个条件生成式策略。

把未来目标回报、状态和动作按时间交错成序列，因果 Transformer 用过去上下文预测当前动作。训练直接拟合数据动作；执行后减去已经获得的奖励，再把更新后的目标回报与新状态送回模型。实验用 Atari、Gym 与长时序任务检验这个条件生成式策略。

[本篇星系](../decision-transformer.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/decision-transformer.md) · [原文依据](https://proceedings.neurips.cc/paper_files/paper/2021/hash/7f489f642a0ddb10272b5c31057f0663-Abstract.html)
