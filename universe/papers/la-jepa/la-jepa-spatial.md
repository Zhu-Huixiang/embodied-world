# 平均与拼接都减少token，但保留信息不同 · La-JEPA

2×2平均压缩存储；patch grouping把邻域特征拼进更宽token。

LIBERO保留均值池化，RoboTwin采用patch grouping。两者token减少，拼接不丢原特征值却保留全尺寸特征存储；文中相关比较还涉及数据split与投影，不能当完全单因素因果收益。

[本篇星系](../la-jepa.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/la-jepa.md) · [原文依据](https://arxiv.org/pdf/2611.08156v1)
