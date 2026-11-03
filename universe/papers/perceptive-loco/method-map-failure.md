# 高度图错误有不同来源 · Perceptive Locomotion

深度测量、地图表示、机器人定位和遮挡都会使高度样本不完整或失真。

控制器要处理的不只是独立小噪声：反光可产生假坑，雪地可能无点，树枝被投到地面高度场，脚滑又会让配准地图整体漂移。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#22-外感知会怎样出错)

继续拆：[2.5D地图只给每个平面位置一个高度](method-map-geometry.md) · [脚滑会反过来弄坏地图](method-pose-map-coupling.md)。

[本篇星系](../perceptive-loco.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md) · [原文依据](https://leggedrobotics.github.io/rl-perceptiveloco/assets/pdf/wild_anymal.pdf)
