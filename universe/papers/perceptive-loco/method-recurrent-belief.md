# 两层GRU积累接触与感知历史 · Perceptive Locomotion

信念编码器用两层各50隐藏单元的GRU整合本体、带噪外感特征和上一步隐状态。

得到的循环表征可以在足离地后保留刚才的接触线索；隐藏状态随运行更新，神经网络权重仍保持已训练值。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#48-信念编码器门控与记忆分别做什么)

继续拆：[门控调节外感特征的捷径](method-gated-skip.md) · [辅助解码器让内部表征有可检查目标](method-auxiliary-decoder.md)。

[本篇星系](../perceptive-loco.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md) · [原文依据](https://leggedrobotics.github.io/rl-perceptiveloco/assets/pdf/wild_anymal.pdf)
