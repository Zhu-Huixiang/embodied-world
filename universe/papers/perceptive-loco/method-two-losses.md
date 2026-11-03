# 动作模仿与环境重建共同监督 · Perceptive Locomotion

学生最小化动作平方差Lbc，并以0.5权重加入无噪高度和特权状态的重建误差Lre。

主文说belief要捕获教师特征所含的控制信息，但明确训练损失只有这两类；没有据此增加一个独立的教师潜变量均方误差。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#46-学生训练模仿动作也重建环境)

[本篇星系](../perceptive-loco.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md) · [原文依据](https://leggedrobotics.github.io/rl-perceptiveloco/assets/pdf/wild_anymal.pdf)
