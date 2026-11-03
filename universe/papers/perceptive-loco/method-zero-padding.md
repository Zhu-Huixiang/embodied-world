# 96维外感必须补到120维才能相加 · Perceptive Locomotion

外感特征和门值都是96维，循环分支产生120维belief候选。

S6明确对门控后的外感结果做零填充再相加；这24个补零维度不等于运行时直接得到了24维特权真值。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#48-信念编码器门控与记忆分别做什么)

[本篇星系](../perceptive-loco.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md) · [原文依据](https://leggedrobotics.github.io/rl-perceptiveloco/assets/pdf/wild_anymal.pdf)
