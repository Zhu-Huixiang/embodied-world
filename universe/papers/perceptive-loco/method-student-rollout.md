# 在学生自己访问的状态上向教师学 · Perceptive Locomotion

学生带噪运行产生轨迹，教师在同一仿真状态和命令下提供参考动作。

若只训练理想教师轨迹，学生小错误带来的后续状态可能缺乏监督；这里通过学生rollout覆盖自己的偏离。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#46-学生训练模仿动作也重建环境)

继续拆：[动作模仿与环境重建共同监督](method-two-losses.md) · [沿用教师主网络来初始化学生](method-student-initialization.md) · [截断梯度长度不是记忆保质期](method-truncated-gradient.md)。

[本篇星系](../perceptive-loco.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md) · [原文依据](https://leggedrobotics.github.io/rl-perceptiveloco/assets/pdf/wild_anymal.pdf)
