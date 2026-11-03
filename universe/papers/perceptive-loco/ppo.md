# PPO 与并行模拟 · Perceptive Locomotion

用受约束的策略更新与大量模拟轨迹训练控制；并行度改变每轮数据和训练开销。

PPO用旧策略采集的轨迹估计动作优势，再通过裁剪目标更新策略；并行环境提供多条轨迹，硬件与模拟器决定采样开销。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#43-教师策略它先拿到哪些答案)

[跨论文技术入口](../../concepts/ppo.md)

[本篇星系](../perceptive-loco.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md) · [原文依据](https://www.science.org/doi/10.1126/scirobotics.abk2822)
