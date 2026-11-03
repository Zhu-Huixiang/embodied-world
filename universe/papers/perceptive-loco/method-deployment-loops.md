# 20Hz地图与50Hz动作异步衔接 · Perceptive Locomotion

GPU地图管线以20Hz整合点云，策略以50Hz从最新地图采样并生成动作。

每次策略调用不必等待一张新地图；空白采样处填随机值。执行仍持续接回本体观测与GRU记忆，形成闭环。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#49-部署20-hz-地图接上-50-hz-控制)

继续拆：[同一高度接口连接两种传感配置](method-sensor-variants.md)。

[本篇星系](../perceptive-loco.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md) · [原文依据](https://leggedrobotics.github.io/rl-perceptiveloco/assets/pdf/wild_anymal.pdf)
