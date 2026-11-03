# 391维教师输入与341维学生输入 · Perceptive Locomotion

TableS3列出本体133维、地高208维和特权50维；学生去掉特权并对地高加噪。

本体包括命令、姿态、身体速度、当前关节、历史关节与目标以及CPG相位。历史是输入的一部分，不能把策略称为只看当前帧。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#44-观察与动作从-391-个数到-12-个关节目标)

继续拆：[每脚五圈共52个高度样本](method-height-rings.md) · [接触与扰动真值只在训练侧可见](method-privileged-input.md)。

[本篇星系](../perceptive-loco.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md) · [原文依据](https://leggedrobotics.github.io/rl-perceptiveloco/assets/pdf/wild_anymal.pdf)
