# SayCan 星系

Do As I Can, Not As I Say: Grounding Language in Robotic Affordances

**导读** · 视觉语言动作模型 VLA

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/saycan.md) · [原文](https://proceedings.mlr.press/v205/ichter23a.html) · [评分卡](../../leaderboard/papers/saycan/README.md)

高层指令与已执行步骤送给语言模型，为每个候选技能估计它对任务的适用性；技能价值函数再估计当前场景下的执行成功可能。两者合并后选择技能、实际执行并把步骤加入上下文，直到选出结束。原文分开报告计划与执行，因而能看清语言推理和物理技能各自卡在哪里。

## 技术挂点

- [分层技能与计划](../concepts/skills.md)：高层选择目标或技能，低层负责具体执行，层次之间有明确接口。

- [价值估计与校准](../concepts/value.md)：估计未来累积收益，再用保守、分位或参考价值等约束减少误导。

- [零样本任务接口](../concepts/zero-shot.md)：不用目标数据集训练样本拟合分类头，而用任务描述等已有信息直接构造预测接口。

## 本篇行星与卫星

- [分层技能与计划](saycan/skills.md) · 初读挂点
- [价值估计与校准](saycan/value.md) · 初读挂点
- [零样本任务接口](saycan/zero-shot.md) · 初读挂点
- [本篇方法链路](saycan/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
