# Ctrl-World 星系

Ctrl-World: A Controllable Generative World Model for Robot Manipulation

**导读** · 世界模型与模型强化学习

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/ctrl-world.md) · [原文](https://proceedings.iclr.cc/paper_files/paper/2026/hash/0ae94013da7cd459402fd77874e09ee3-Abstract-Conference.html) · [评分卡](../../leaderboard/papers/ctrl-world/README.md)

1.5B SVD初始化，多相机token联合生成；稀疏历史图像带机器人姿态通过逐帧cross-attention检索；未来动作转换笛卡尔姿态后逐帧条件化。策略在模型里闭环rollout，人工筛成功轨迹再微调VLA。

## 技术挂点

- [视频时序生成](../concepts/video.md)：同时表达画面内容与时间变化，用历史与条件产生连续帧。

- [动作条件动力学](../concepts/dynamics.md)：以当前状态和动作预测下一状态或分布，建立“做这个动作会发生什么”的计算接口。

- [闭环滚动与历史偏移](../concepts/rollout.md)：重复预测、执行或生成，把新观测或模型历史接回后续计算。

## 本篇行星与卫星

- [视频时序生成](ctrl-world/video.md) · 初读挂点
- [动作条件动力学](ctrl-world/dynamics.md) · 初读挂点
- [闭环滚动与历史偏移](ctrl-world/rollout.md) · 初读挂点
- [本篇方法链路](ctrl-world/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
