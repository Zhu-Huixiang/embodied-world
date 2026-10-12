# RT-2 星系

RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control

**导读** · 视觉语言动作模型 VLA

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/rt2.md) · [原文](https://proceedings.mlr.press/v229/zitkovich23a.html) · [评分卡](../../leaderboard/papers/rt2/README.md)

把机器人动作写成语言模型词表内的编号，将机器人示范与视觉语言任务共同训练以迁移网络语义。

## 技术挂点

- [离散编码与量化](../concepts/quantization.md)：把连续向量或信号映射到有限码。动作、视频潜变量与世界模型状态都可能采用这种表示，码本和训练目标各不相同。

- [跨本体数据](../concepts/cross-body.md)：从多个机器人或人类收集经验，通过动作/观测适配接到共享学习系统。

- [因果序列建模](../concepts/causal.md)：通过遮罩只让位置读取允许的历史，避免训练时看到运行时不存在的未来。

## 本篇行星与卫星

- [离散编码与量化](rt2/quantization.md) · 初读挂点
- [跨本体数据](rt2/cross-body.md) · 初读挂点
- [因果序列建模](rt2/causal.md) · 初读挂点
- [本篇方法链路](rt2/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
