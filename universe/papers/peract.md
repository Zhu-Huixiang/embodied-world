# PerAct 星系

Perceiver-Actor: A Multi-Task Transformer for Robotic Manipulation

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/peract.md) · [原文](https://proceedings.mlr.press/v205/shridhar23a.html) · [评分卡](../../leaderboard/papers/peract/README.md)

RGB-D 重建为三维体素网格，体素 patch 与语言向量组成序列；Perceiver 用少量 latent 承接长输入。输出逐体素特征后检测下一关键动作的位置，并预测离散旋转、夹爪及碰撞选项，交由运动规划器执行。网格把观测位置和动作位置对齐，原文再比较图像回归、3D 卷积与多任务少示范性能。

## 技术挂点

- [点云与三维体素](../concepts/point-cloud.md)：点云用三维点记录几何，网络从点的位置与特征构造空间表示。

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。

## 本篇行星与卫星

- [点云与三维体素](peract/point-cloud.md) · 初读挂点
- [注意力](peract/attention.md) · 初读挂点
- [空间表示](peract/spatial.md) · 初读挂点
- [本篇方法链路](peract/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
