# 四项模仿奖励 · DeepMimic

姿态、角速度、手脚末端、质心分别比较参考并指数压缩。

权重.65/.1/.15/.1；各误差单位不同，指数尺度决定敏感性。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md#53-奖励)

继续拆：[四元数相对转角](quaternion-pose-error.md) · [参考角速度的差分](finite-difference-velocity.md) · [手脚世界位置误差](end-effector-world-error.md) · [质心位置误差](center-of-mass-error.md) · [模仿和任务的加权](task-imitation-mixture.md)。

[本篇星系](../deepmimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md) · [原文依据](https://xbpeng.github.io/projects/DeepMimic/DeepMimic_2018.pdf)
