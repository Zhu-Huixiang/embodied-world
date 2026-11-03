# 仿真动力学与学习到的执行器模型 · Perceptive Locomotion

训练在RaiSim中并行模拟ANYmal-C，结合执行器模型减少仿真与现实的差别。

环境还包含参数化起伏、离散台阶、方块与不同楼梯；这是在仿真中产生控制训练数据，不是从真实登山视频模仿。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#42-仿真环境地形与课程)

继续拆：[用箱体楼梯堵住仿真几何捷径](method-stair-geometry.md) · [随机化身体与接触条件](method-randomization.md) · [不良状态触发训练终止](method-termination.md) · [地形课程与代价课程分开推进](method-curriculum.md)。

[本篇星系](../perceptive-loco.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md) · [原文依据](https://leggedrobotics.github.io/rl-perceptiveloco/assets/pdf/wild_anymal.pdf)
