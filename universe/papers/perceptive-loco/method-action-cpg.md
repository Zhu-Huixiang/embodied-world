# 16维动作经CPG与IK变成目标角 · Perceptive Locomotion

策略输出四维相位偏移和十二维关节残差，名义足轨迹经解析逆运动学后再加残差。

相位调节落在摆动还是支撑周期，关节残差调整具体姿态。最终十二关节目标与网络的十六维动作是两个接口。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#44-观察与动作从-391-个数到-12-个关节目标)

继续拆：[名义摆腿轨迹是可修正的脚端基准](method-nominal-trajectory.md)。

[本篇星系](../perceptive-loco.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md) · [原文依据](https://leggedrobotics.github.io/rl-perceptiveloco/assets/pdf/wild_anymal.pdf)
