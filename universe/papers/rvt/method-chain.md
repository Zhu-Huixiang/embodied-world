# 本篇方法链路 · RVT

RGB-D 先变成点云，再从机器人工作区周围的虚拟相机重渲染多张视图；Transformer 在视图内及视图间聚合信息。多视图动作热图反投影得到夹爪位置，其他头预测姿态与夹爪状态。原文把成功率、训练达到相同性能所需时间和推理速度分别与 PerAct 对比，并展示真实少示范操作。

RGB-D 先变成点云，再从机器人工作区周围的虚拟相机重渲染多张视图；Transformer 在视图内及视图间聚合信息。多视图动作热图反投影得到夹爪位置，其他头预测姿态与夹爪状态。原文把成功率、训练达到相同性能所需时间和推理速度分别与 PerAct 对比，并展示真实少示范操作。

[本篇星系](../rvt.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/rvt.md) · [原文依据](https://proceedings.mlr.press/v229/goyal23a.html)
