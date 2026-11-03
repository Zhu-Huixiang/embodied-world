# 每轮并行采样不等于总训练时长 · Perceptive Locomotion

教师每轮1000环境各250步，控制频率50Hz，合计每轮250000个仿真步。

附录给PPO裁剪比0.2、折扣0.996、学习率5e-4。这些是每轮配置，不能据此补出论文没有报告的总训练步数或墙钟时间。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#43-教师策略它先拿到哪些答案)

[本篇星系](../perceptive-loco.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md) · [原文依据](https://leggedrobotics.github.io/rl-perceptiveloco/assets/pdf/wild_anymal.pdf)
