# Open X-Embodiment 星系

Open X-Embodiment: Robotic Learning Datasets and RT-X Models

**导读** · 视觉语言动作模型 VLA

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/rtx.md) · [原文](https://ieeexplore.ieee.org/document/10611477) · [评分卡](../../leaderboard/papers/rtx/README.md)

先把各实验室的轨迹变成统一数据格式，并以夹爪参考系中的位置、姿态和夹爪开合统一动作接口；未使用的动作分量按数据约定处理。RT-1-X 和 RT-2-X 在这个混合数据上训练，再与各机器人自己的专用数据策略比较。它检验的不是同一机器人多收点数据，而是别的机器人经验能否改善当前机器人。

## 技术挂点

- [跨本体数据](../concepts/cross-body.md)：从多个机器人或人类收集经验，通过动作/观测适配接到共享学习系统。

- [机器人数据与评测](../concepts/data.md)：统一观测、动作、任务与评测条件，判断数据多样性如何影响泛化。

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

## 本篇行星与卫星

- [跨本体数据](rtx/cross-body.md) · 初读挂点
- [机器人数据与评测](rtx/data.md) · 初读挂点
- [动作表示](rtx/action.md) · 初读挂点
- [本篇方法链路](rtx/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
