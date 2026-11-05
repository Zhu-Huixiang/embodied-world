# DROID八步动作历史 · DreamFree

历史动作抑制闭环中的意外重新张夹爪。

输入顺序为当前状态、过去8动作、加噪未来动作；历史缺项mask，训练时状态与整段历史分别以0.2概率drop；只有DROID启用。

[本篇星系](../dreamfree.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamfree.md) · [原文依据](https://arxiv.org/pdf/2611.04527v1)
