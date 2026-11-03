# 教师先用仿真真值学控制 · Perceptive Locomotion

教师读取本体观测、无噪地高和接触、摩擦、扰动等特权状态，以PPO学习跟随速度命令。

命令包含机体坐标系下的前向、侧向与yaw速度。真值帮助先获得动作参考，部署学生要从可感知输入补足这些信息。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#43-教师策略它先拿到哪些答案)

继续拆：[两路压缩后再接动作网络](method-teacher-latents.md) · [每轮并行采样不等于总训练时长](method-training-budget.md)。

[本篇星系](../perceptive-loco.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md) · [原文依据](https://leggedrobotics.github.io/rl-perceptiveloco/assets/pdf/wild_anymal.pdf)
