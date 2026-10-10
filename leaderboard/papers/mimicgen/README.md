# MimicGen: A Data Generation System for Scalable Robot Learning using Human Demonstrations

本版阅读优先顺序：83；综合分：81.3 / 100；已评分权重：100%。

[原文](https://proceedings.mlr.press/v229/mandlekar23a.html) · [PDF](https://proceedings.mlr.press/v229/mandlekar23a/mandlekar23a.pdf) · [阅读卡片](../../../library/mimicgen.md)

## 机制简析

源示范按对象中心子任务切段；新场景中选择源段，按对象的新位姿变换末端轨迹，再拼接并实际执行。执行成功才把状态和动作加入生成数据，而不是只复制一组数学坐标。原文逐步扩大初始状态分布、替换物体与机械臂，并比较生成示范和追加同量人类示范的策略表现。

带着这个问题读：把十条示范扩成上千条，什么时候是有用的新数据，什么时候只是机械复制？

初读判断：CoRL PDF 明确动作和对象假设，提供跨任务/模拟器/硬件生成、初始分布和示范质量研究；项目公开生成代码、数据和环境，复用价值很高。

## 七维评分

![七维雷达：加载时展开一次，随后静止](radar.gif)

打开时从中心展开一次，结束后保持最终形状。[直接查看静态图](radar.svg)。加载与再次打开的播放时机取决于浏览器缓存。

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 刊会质量 | 90.0 | 30% |
| 创新性 | 91 | 20% |
| 实验与证据 | 94 | 20% |
| 学术影响 | 22.4 | 10% |
| 近期关注 | 11.1 | 5% |
| 复用价值 | 98 | 8% |
| 阅读价值 | 95 | 7% |

刊会依据：[CoRL 2023](../../../venues/CoRL/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v229/mandlekar23a.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：MimicGen: A Data Generation System for Scalable Robot Learning using Human Demonstrations。累计被引 5，2025–2026 被引 1；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4387994700) · [文献计量条目](https://openalex.org/W4387994700)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
