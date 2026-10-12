# ACT / ALOHA 星系

Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/act.md) · [原文](https://www.roboticsproceedings.org/rss19/p016.html) · [评分卡](../../leaderboard/papers/act/README.md)

把一段动作联合预测，条件变分自编码器吸收示范差异，时间集成融合重叠预测减轻误差积累。

## 技术挂点

- [变分自编码器 VAE](../concepts/vae.md)：编码器描述潜变量分布，解码器从潜变量重建样本，用重建与分布正则共同训练。

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。

- [行为克隆](../concepts/bc.md)：直接监督观测到动作的映射，不必在每次更新中根据奖励搜索。

## 本篇行星与卫星

- [变分自编码器 VAE](act/vae.md) · 初读挂点
- [动作块](act/chunk.md) · 初读挂点
- [行为克隆](act/bc.md) · 初读挂点
- [本篇方法链路](act/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
