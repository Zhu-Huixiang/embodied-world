# 本篇方法链路 · Consistency Models

学习一个映射，使概率流 ODE 同一轨迹上的不同噪声点都输出同一个干净样本。蒸馏版由教师扩散模型和求解器产生相邻轨迹点，训练版则直接通过相邻噪声尺度的一致性约束学习。原文在标准图像数据集比较一步、少步生成和编辑，机器人策略将同类映射用于压缩动作采样延迟。

学习一个映射，使概率流 ODE 同一轨迹上的不同噪声点都输出同一个干净样本。蒸馏版由教师扩散模型和求解器产生相邻轨迹点，训练版则直接通过相邻噪声尺度的一致性约束学习。原文在标准图像数据集比较一步、少步生成和编辑，机器人策略将同类映射用于压缩动作采样延迟。

[本篇星系](../consistency-models.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/consistency-models.md) · [原文依据](https://proceedings.mlr.press/v202/song23a.html)
