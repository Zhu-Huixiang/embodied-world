# 软泡沫触地后向下修正内部地形 · Perceptive Locomotion

泡沫外观像实心台阶，接触时下陷，循环表征的解码高度随之下降。

红点是输入高度，蓝点是内省解码出的估计。离地后估计仍保留，显示历史信息进入表征，而不是每一帧完全重置。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#24-接触之后内部地形怎样改写)

继续拆：[透明台阶接触后向上修正](experiment-transparent.md) · [遮挡传感器后退回接触反应](experiment-blind.md) · [摩擦曲线是内省解码结果](experiment-friction-decoding.md)。

[本篇星系](../perceptive-loco.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md) · [原文依据](https://leggedrobotics.github.io/rl-perceptiveloco/assets/pdf/wild_anymal.pdf)
