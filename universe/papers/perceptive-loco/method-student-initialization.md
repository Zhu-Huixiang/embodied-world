# 沿用教师主网络来初始化学生 · Perceptive Locomotion

教师与学生的动作MLP结构相同，可用训练好的教师权重初始化以加速学习。

学生多了循环信念编码器与感知噪声训练；初始化是训练起点，不应解读为整套学生动作网络在第二阶段始终冻结。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#46-学生训练模仿动作也重建环境)

[本篇星系](../perceptive-loco.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md) · [原文依据](https://leggedrobotics.github.io/rl-perceptiveloco/assets/pdf/wild_anymal.pdf)
