# RVT 星系

RVT: Robotic View Transformer for 3D Object Manipulation

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/rvt.md) · [原文](https://proceedings.mlr.press/v229/goyal23a.html) · [评分卡](../../leaderboard/papers/rvt/README.md)

RGB-D 先变成点云，再从机器人工作区周围的虚拟相机重渲染多张视图；Transformer 在视图内及视图间聚合信息。多视图动作热图反投影得到夹爪位置，其他头预测姿态与夹爪状态。原文把成功率、训练达到相同性能所需时间和推理速度分别与 PerAct 对比，并展示真实少示范操作。

## 技术挂点

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。

- [点云与三维体素](../concepts/point-cloud.md)：点云用三维点记录几何，网络从点的位置与特征构造空间表示。

## 本篇行星与卫星

- [空间表示](rvt/spatial.md) · 初读挂点
- [注意力](rvt/attention.md) · 初读挂点
- [点云与三维体素](rvt/point-cloud.md) · 初读挂点
- [本篇方法链路](rvt/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
