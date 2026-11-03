# 门控调节外感特征的捷径 · Perceptive Locomotion

96维sigmoid门值逐元素乘外感特征，经零填充后加入120维循环分支输出。

这不是拿两个完整控制器做硬切换；GRU本身仍接收外感，门控改变的是直接进入最终belief的外感skip强度。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#48-信念编码器门控与记忆分别做什么)

继续拆：[96维外感必须补到120维才能相加](method-zero-padding.md)。

[本篇星系](../perceptive-loco.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md) · [原文依据](https://leggedrobotics.github.io/rl-perceptiveloco/assets/pdf/wild_anymal.pdf)
