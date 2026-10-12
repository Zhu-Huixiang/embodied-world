# 一致性生成

让同一生成轨迹上的不同噪声状态映射到相同干净目标，用于一步或少步生成。

一致性策略把减少采样调用与实际动作成功率放在一起比较。

分类上层：[扩散去噪](diffusion.md)。

## 哪些论文用到或讨论它

- [Consistency Policy](../papers/consistency-policy.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss20/p071.html)
- [Consistency Models](../papers/consistency-models.md) · 机制导读 · [原文](https://proceedings.mlr.press/v202/song23a.html)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
