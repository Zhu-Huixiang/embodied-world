# 冻结骨干的一次前向 · GAR

图像、指令和机器人状态经冻结教师产生动作读出特征。

固定噪声ε*与t=0输入动作Transformer；均值、协方差和命令头共用最终速度投影之前的特征，教师参数保持冻结。

继续拆：[均值与协方差读出](heads.md) · [离散命令的probit读出](binary.md)。

[本篇星系](../gar.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/gar.md) · [原文依据](https://arxiv.org/pdf/2610.40271v1)
