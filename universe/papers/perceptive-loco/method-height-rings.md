# 每脚五圈共52个高度样本 · Perceptive Locomotion

五个半径为0.08、0.16、0.26、0.36、0.48米，对应6、8、10、12、16个采样点。

四脚合计208个高度值，围绕各足取样；策略读的是这些局部地形扫描，不是把整个地图每个像素直接输入动作网络。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#44-观察与动作从-391-个数到-12-个关节目标)

[本篇星系](../perceptive-loco.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md) · [原文依据](https://leggedrobotics.github.io/rl-perceptiveloco/assets/pdf/wild_anymal.pdf)
