# OmniH2O: Universal and Dexterous Human-to-Humanoid Whole-Body Teleoperation and Learning

本版阅读优先顺序：91；综合分：76.8 / 100；已评分权重：100%。

[原文](https://proceedings.mlr.press/v270/he25b.html) · [PDF](https://raw.githubusercontent.com/mlresearch/v270/main/assets/he25b/he25b.pdf) · [阅读卡片](../../../library/omnih2o.md)

## 机制简析

把不同遥操作方式转换成运动学姿态目标，再交给跟踪控制器。特权教师在模拟中学大规模动作，学生用本体历史与稀疏目标通过 DAgger 模仿教师，输出可部署的动作；手部另接姿态到关节控制。原文验证模拟和实机跟踪、不同控制入口及采集示范后的自主技能。

带着这个问题读：只有头和双手目标，为什么还能指挥整个身体并收集自主学习数据？

初读判断：有大规模跟踪、实机指标与 DAgger/历史/目标点消融，统一接口和公开数据支持后续复用。

## 七维评分

![七维雷达：加载时展开一次，随后静止](radar.gif)

打开时从中心展开一次，结束后保持最终形状。[直接查看静态图](radar.svg)。加载与再次打开的播放时机取决于浏览器缓存。

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 刊会质量 | 90.0 | 30% |
| 创新性 | 89 | 20% |
| 实验与证据 | 90 | 20% |
| 学术影响 | 0.0 | 10% |
| 近期关注 | 0.0 | 5% |
| 复用价值 | 93 | 8% |
| 阅读价值 | 94 | 7% |

刊会依据：[CoRL 2024](../../../venues/CoRL/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v270/he25b.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：OmniH2O: Universal and Dexterous Human-to-Humanoid Whole-Body Teleoperation and Learning。累计被引 0，2025–2026 被引 0；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W4399695336) · [文献计量条目](https://openalex.org/W4399695336)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
