# Cal-QL: Calibrated Offline RL Pre-Training for Efficient Online Fine-Tuning

本版阅读优先顺序：72；综合分：82.9 / 100；已评分权重：100%。

[原文](https://proceedings.neurips.cc/paper_files/paper/2023/hash/c44a04289beaf0a7d968a94066a1d696-Abstract-Conference.html) · [PDF](https://proceedings.neurips.cc/paper_files/paper/2023/file/c44a04289beaf0a7d968a94066a1d696-Paper-Conference.pdf) · [阅读卡片](../../../library/cal-ql.md)

## 机制简析

Cal-QL 保留 CQL 的保守价值学习，同时把学习策略的价值锚定在一个可估计参考策略的价值之上。这样在线新数据进入时，低估的旧 Q 不至于诱导策略先丢掉离线技能。原文分别分析初期遗忘、价值尺度变化，并在导航、操作和图像输入微调任务上比较。

带着这个问题读：离线训练把 Q 压得太低，为什么一上真环境反而会先忘掉已有技能？

初读判断：先诊断再设计算法，含多个离线到在线域、理论条件、基线和校准消融，适合作为机器人预训练后的 RL 入门。

## 七维评分

![七维雷达：加载时展开一次，随后静止](radar.gif)

打开时从中心展开一次，结束后保持最终形状。[直接查看静态图](radar.svg)。加载与再次打开的播放时机取决于浏览器缓存。

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 刊会质量 | 95.0 | 30% |
| 创新性 | 87 | 20% |
| 实验与证据 | 89 | 20% |
| 学术影响 | 33.8 | 10% |
| 近期关注 | 43.6 | 5% |
| 复用价值 | 90 | 8% |
| 阅读价值 | 92 | 7% |

刊会依据：[NeurIPS 2023](../../../venues/NeurIPS/README.md)，正式出处见[出版/原文记录](https://proceedings.neurips.cc/paper_files/paper/2023/hash/c44a04289beaf0a7d968a94066a1d696-Abstract-Conference.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：正式刊会版本；OpenAlex题目：Cal-QL: Calibrated Offline RL Pre-Training for Efficient Online Fine-Tuning。累计被引 14，2025–2026 被引 14；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W7133245541) · [文献计量条目](https://openalex.org/W7133245541)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
