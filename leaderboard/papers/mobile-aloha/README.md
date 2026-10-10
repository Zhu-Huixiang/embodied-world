# Mobile ALOHA: Learning Bimanual Mobile Manipulation using Low-Cost Whole-Body Teleoperation

本版阅读优先顺序：69；综合分：83.2 / 100；已评分权重：100%。

[原文](https://proceedings.mlr.press/v270/fu25b.html) · [PDF](https://raw.githubusercontent.com/mlresearch/v270/main/assets/fu25b/fu25b.pdf) · [阅读卡片](../../../library/mobile-aloha.md)

## 机制简析

把双臂关节位置与底盘线/角速度拼成统一动作，遥操作同时记录手臂与底盘；行为克隆直接预测整套动作。训练混入已有静态 ALOHA 示范，检验不同任务、臂安装位置和场景之间的正迁移。原文把自治策略执行与人类遥操作采集分开，比较联合训练和只用移动数据的任务表现。

带着这个问题读：桌面双臂经验为什么能帮会移动的机器人做饭、开柜子和坐电梯？

初读判断：CoRL 正式稿与首版方法给出真实长程移动任务和联合训练对照，开放软硬件便于复用；视觉演示具有传播价值，评分仍以自治任务评估而非视频震撼程度为依据。

## 七维评分

![七维雷达：加载时展开一次，随后静止](radar.gif)

打开时从中心展开一次，结束后保持最终形状。[直接查看静态图](radar.svg)。加载与再次打开的播放时机取决于浏览器缓存。

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 刊会质量 | 90.0 | 30% |
| 创新性 | 87 | 20% |
| 实验与证据 | 90 | 20% |
| 学术影响 | 42.9 | 10% |
| 近期关注 | 44.6 | 5% |
| 复用价值 | 93 | 8% |
| 阅读价值 | 97 | 7% |

刊会依据：[CoRL 2024](../../../venues/CoRL/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v270/fu25b.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：Mobile ALOHA: Learning Bimanual Mobile Manipulation with Low-Cost Whole-Body Teleoperation。累计被引 30，2025–2026 被引 15；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4390635563) · [文献计量条目](https://openalex.org/W4390635563)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
