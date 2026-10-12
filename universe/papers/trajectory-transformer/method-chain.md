# 本篇方法链路 · Trajectory Transformer

把状态和动作各维离散化，与奖励串成 token，Transformer 联合学习整段轨迹的概率。规划时用 beam search 保留高回报候选轨迹，执行第一步后重新搜索；稀疏长时序任务还可以接 IQL 的 Q 值做搜索启发。原文同时检查长预测误差、模仿、目标到达与离线 RL。

把状态和动作各维离散化，与奖励串成 token，Transformer 联合学习整段轨迹的概率。规划时用 beam search 保留高回报候选轨迹，执行第一步后重新搜索；稀疏长时序任务还可以接 IQL 的 Q 值做搜索启发。原文同时检查长预测误差、模仿、目标到达与离线 RL。

[本篇星系](../trajectory-transformer.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/trajectory-transformer.md) · [原文依据](https://proceedings.neurips.cc/paper_files/paper/2021/hash/099fe6b0b444c23836c4a5d07346082b-Abstract.html)
