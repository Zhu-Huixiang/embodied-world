# 本篇方法链路 · DayDreamer

真实机器人持续把轨迹写入经验回放，学习线程更新潜空间世界模型，再用模型想象的轨迹训练策略和值函数。异步 actor 与 learner 把快速执行和较慢训练拆开，避免每次梯度更新卡住机器人控制。原文用四足、两种机械臂和轮式机器人检查同一算法的在线学习能力。

真实机器人持续把轨迹写入经验回放，学习线程更新潜空间世界模型，再用模型想象的轨迹训练策略和值函数。异步 actor 与 learner 把快速执行和较慢训练拆开，避免每次梯度更新卡住机器人控制。原文用四足、两种机械臂和轮式机器人检查同一算法的在线学习能力。

[本篇星系](../daydreamer.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/daydreamer.md) · [原文依据](https://proceedings.mlr.press/v205/wu23c.html)
