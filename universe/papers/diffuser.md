# Diffuser 星系

Planning with Diffusion for Flexible Behavior Synthesis

**导读** · 世界动作模型

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/diffuser.md) · [原文](https://proceedings.mlr.press/v162/janner22a.html) · [评分卡](../../leaderboard/papers/diffuser/README.md)

Diffuser 学习整段状态—动作轨迹的去噪过程，反复修正所有规划时刻，而不是单步滚动一个动力学模型。奖励梯度可以引导去噪，固定起点或终点则像图像补全那样锁住轨迹部分。论文在长时序与灵活测试条件下比较规划效果，并区分扩散步和环境时间步。

## 技术挂点

- [扩散去噪](../concepts/diffusion.md)：训练网络从带噪对象估计噪声或干净目标，生成时从噪声开始迭代恢复样本。

- [树搜索与轨迹搜索](../concepts/search.md)：展开候选动作或轨迹，用预测价值挑选可执行方案。

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

## 本篇行星与卫星

- [扩散去噪](diffuser/diffusion.md) · 初读挂点
- [树搜索与轨迹搜索](diffuser/search.md) · 初读挂点
- [动作表示](diffuser/action.md) · 初读挂点
- [本篇方法链路](diffuser/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
