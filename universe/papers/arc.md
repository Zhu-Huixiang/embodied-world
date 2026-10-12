# ARC 星系

ARC: A Reasoning Recipe for Robot Foundation Models

**导读** · 视觉语言动作模型 VLA

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/arc.md) · [原文](https://arxiv.org/abs/2610.12386v1) · [评分卡](../../leaderboard/papers/arc/README.md)

给现有示范自动添“下一动作为什么合适、会造成什么”的推理轨迹，再按 VLA/WAM 架构适配推理与动作输出。

## 技术挂点

- [因果序列建模](../concepts/causal.md)：通过遮罩只让位置读取允许的历史，避免训练时看到运行时不存在的未来。

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

- [世界动作联合建模](../concepts/wam.md)：把未来状态或视频与动作放进联合条件生成过程，让视觉动态和行动相互约束。

## 本篇行星与卫星

- [因果序列建模](arc/causal.md) · 初读挂点
- [动作表示](arc/action.md) · 初读挂点
- [世界动作联合建模](arc/wam.md) · 初读挂点
- [本篇方法链路](arc/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
