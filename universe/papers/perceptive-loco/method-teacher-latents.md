# 两路压缩后再接动作网络 · Perceptive Locomotion

每脚52个高度样本压成24维，四脚拼为96维；50维特权状态另压成24维。

这120维环境特征与133维本体观测拼接成253维输入，进入隐藏宽度256、160、128的动作MLP；原始391维与压缩后253维不能混称。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#44-观察与动作从-391-个数到-12-个关节目标)

[本篇星系](../perceptive-loco.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md) · [原文依据](https://leggedrobotics.github.io/rl-perceptiveloco/assets/pdf/wild_anymal.pdf)
