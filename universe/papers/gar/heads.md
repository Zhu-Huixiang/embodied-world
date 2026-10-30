# 均值与协方差读出 · GAR

仿射均值修正与池化MLP分别预测动作矩。

均值头修正教师单步输出；协方差头跨动作位置池化、使用128单元GELU隐藏层。对角版本输出正方差，全协方差版本输出正对角Cholesky因子。RoboCasa Xiaomi连续维160，GR00T为144变化维及16固定零维。

继续拆：[教师采样目标与数据划分](teacher-targets.md) · [一步采样与闭式似然](sampling.md)。

[本篇星系](../gar.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/gar.md) · [原文依据](https://arxiv.org/pdf/2610.40271v1)
