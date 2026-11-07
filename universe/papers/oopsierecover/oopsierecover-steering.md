# 冻结策略提候选，纠正规则做筛选 · OopsieRecover

从VLA采样K个长度H的动作块，预测它们会怎样移动点集。

Eq7–8沿预测轨迹累积折扣代价并选最小者；可补cardinal actions增加候选多样性，多条规则同时触发时加权成本。候选中没有有效动作时无法保证恢复。

继续拆：[仿真预测器和实机预测器要分开看](oopsierecover-dynamics.md)。

[本篇星系](../oopsierecover.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/oopsierecover.md) · [原文依据](https://arxiv.org/pdf/2611.08462v1)
