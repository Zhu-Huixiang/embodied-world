# 把噪声加在位置、高度和不同时间范围 · Perceptive Locomotion

高度样本的平面位置与高度都被扰动，噪声按采样点、足和episode施加。

独立点噪声模拟散点不稳，每脚整体偏移模拟定位漂移或软地面，episode内固定偏移模拟持续误差；另有偶发离群点。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#47-高度噪声故意把地图弄坏)

继续拆：[三种地图质量按60比30比10采样](method-noise-mixture.md) · [学生先学简单地形再加大感知破坏](method-noise-curriculum.md)。

[本篇星系](../perceptive-loco.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md) · [原文依据](https://leggedrobotics.github.io/rl-perceptiveloco/assets/pdf/wild_anymal.pdf)
