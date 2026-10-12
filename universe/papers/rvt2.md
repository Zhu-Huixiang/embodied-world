# RVT-2 星系

RVT-2: Learning Precise Manipulation from Few Demonstrations

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/rvt2.md) · [原文](https://www.roboticsproceedings.org/rss20/p055.html) · [评分卡](../../leaderboard/papers/rvt2/README.md)

第一阶段在全场景虚拟视图中估计目标，第二阶段放大局部区域后预测更精确的位置；旋转预测改用目标位置附近特征，避免同场景多个物体方向冲突。凸上采样、较少视图和高效点云渲染控制计算成本。原文分别做这些部件的消融，并用插头和不同孔径 peg 的实机任务检验精度。

## 技术挂点

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。

- [点云与三维体素](../concepts/point-cloud.md)：点云用三维点记录几何，网络从点的位置与特征构造空间表示。

## 本篇行星与卫星

- [空间表示](rvt2/spatial.md) · 初读挂点
- [注意力](rvt2/attention.md) · 初读挂点
- [点云与三维体素](rvt2/point-cloud.md) · 初读挂点
- [本篇方法链路](rvt2/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
