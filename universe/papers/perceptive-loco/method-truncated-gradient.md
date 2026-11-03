# 截断梯度长度不是记忆保质期 · Perceptive Locomotion

学生每轮300个环境各收400步，循环单元以10步做截断反向传播。

50Hz下10步对应0.2秒，这约束单次梯度传播的时间跨度；它没有证明前向运行中的隐藏状态只能保留0.2秒信息。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#46-学生训练模仿动作也重建环境)

[本篇星系](../perceptive-loco.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md) · [原文依据](https://leggedrobotics.github.io/rl-perceptiveloco/assets/pdf/wild_anymal.pdf)
