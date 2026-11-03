# 特权教师、带噪学生、实机部署 · Perceptive Locomotion

先在仿真中用完整信息训练教师，再监督只有可获取输入的学生，最后将学生移到实机。

第一阶段用奖励学习动作，第二阶段模仿动作并重建环境；运行阶段只做前向推断，不再读取训练真值或做在线梯度更新。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#41-总览与问题定义)

[本篇星系](../perceptive-loco.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md) · [原文依据](https://leggedrobotics.github.io/rl-perceptiveloco/assets/pdf/wild_anymal.pdf)
