# 点云与三维体素

点云用三维点记录几何，网络从点的位置与特征构造空间表示。

点云和体素是不同表示；PerAct 会把观测转成体素，DP3 则编码点云。

分类上层：[空间表示](spatial.md)。

## 哪些论文用到或讨论它

- [DP3](../papers/dp3.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss20/p067.html)
- [PerAct](../papers/peract.md) · 机制导读 · [原文](https://proceedings.mlr.press/v205/shridhar23a.html)
- [RVT](../papers/rvt.md) · 机制导读 · [原文](https://proceedings.mlr.press/v229/goyal23a.html)
- [RVT-2](../papers/rvt2.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss20/p055.html)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
