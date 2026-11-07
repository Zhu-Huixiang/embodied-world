# 目标朝向到力矩闭环 · DeepMimic

策略给关节目标朝向，stable PD给力矩，Bullet推进身体状态反馈给策略。

动作参数不是直接力矩；标准PD直觉式须和实际stable PD实现分开。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md#3-方法总览从参考姿态到物理动作)

继续拆：[参考数据的两条训练通道](reference-two-channels.md) · [轴角与单轴目标动作](joint-target-action.md) · [策略和物理的两级时钟](policy-physics-rates.md)。

[本篇星系](../deepmimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md) · [原文依据](https://xbpeng.github.io/projects/DeepMimic/DeepMimic_2018.pdf)
