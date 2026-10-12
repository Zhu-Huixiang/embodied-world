# RT-1 星系

RT-1: Robotics Transformer for Real-World Control at Scale

**导读** · 视觉语言动作模型 VLA

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/rt1.md) · [原文](https://www.roboticsproceedings.org/rss19/p025.html) · [评分卡](../../leaderboard/papers/rt1/README.md)

图像先经语言条件的 EfficientNet 提取特征，再由 TokenLearner 压成少量视觉 token；Transformer 融合短时历史并输出离散动作。动作同时覆盖机械臂、底盘和停止模式，策略以闭环方式反复读取图像。原文分别检验新指令、干扰物、新背景以及跨机器人数据混合的效果。

## 技术挂点

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。

- [离散编码与量化](../concepts/quantization.md)：把连续向量或信号映射到有限码。动作、视频潜变量与世界模型状态都可能采用这种表示，码本和训练目标各不相同。

- [跨本体数据](../concepts/cross-body.md)：从多个机器人或人类收集经验，通过动作/观测适配接到共享学习系统。

## 本篇行星与卫星

- [注意力](rt1/attention.md) · 初读挂点
- [离散编码与量化](rt1/quantization.md) · 初读挂点
- [跨本体数据](rt1/cross-body.md) · 初读挂点
- [本篇方法链路](rt1/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
