# PPO 与并行模拟 · RMA

用受约束的策略更新与大量模拟轨迹训练控制；并行度改变每轮数据和训练开销。

PPO用旧策略采集的轨迹估计动作优势，再通过裁剪目标更新策略；并行环境提供多条轨迹，硬件与模拟器决定采样开销。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md#42-网络与训练预算)

[跨论文技术入口](../../concepts/ppo.md)

[本篇星系](../rma.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rma-2107.04034/README.md) · [原文依据](https://www.roboticsproceedings.org/rss17/p011.html)
