# 本篇方法链路 · HumanPlus

用人类运动重定向数据在模拟里训练姿态条件的低层控制，再用单 RGB 相机估计操作者姿态，让实机实时跟随。跟随过程中记录机器人双目视觉和全身动作，随后用 Humanoid Imitation Transformer 做监督模仿，得到自主任务策略。原文分别评估遥操作、抗扰和多项自主任务。

用人类运动重定向数据在模拟里训练姿态条件的低层控制，再用单 RGB 相机估计操作者姿态，让实机实时跟随。跟随过程中记录机器人双目视觉和全身动作，随后用 Humanoid Imitation Transformer 做监督模仿，得到自主任务策略。原文分别评估遥操作、抗扰和多项自主任务。

[本篇星系](../humanplus.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/humanplus.md) · [原文依据](https://proceedings.mlr.press/v270/fu25a.html)
