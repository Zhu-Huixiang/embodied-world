# 辅助解码器让内部表征有可检查目标 · Perceptive Locomotion

训练中从循环表征及带噪高度分支重建环境真值，并用于查看内部地形与摩擦估计。

原图decoder接隐藏状态和带噪原始高度；它不在实机动作必经链上。重建结果有助于内省，不能当作额外真实传感器。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#48-信念编码器门控与记忆分别做什么)

[本篇星系](../perceptive-loco.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md) · [原文依据](https://leggedrobotics.github.io/rl-perceptiveloco/assets/pdf/wild_anymal.pdf)
