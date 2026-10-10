# Learning Universal Policies via Text-Guided Video Generation

本版阅读优先顺序：75；综合分：82.9 / 100；已评分权重：100%。

[原文](https://proceedings.neurips.cc/paper_files/paper/2023/hash/1d5b9233ad716a43be5c0d3023cb82d0-Abstract-Conference.html) · [PDF](https://proceedings.neurips.cc/paper_files/paper/2023/file/1d5b9233ad716a43be5c0d3023cb82d0-Paper-Conference.pdf) · [阅读卡片](../../../library/unipi.md)

## 机制简析

当前图像和文字任务条件送入视频扩散模型，生成未来画面序列作为计划；逆动力学模型再从相邻或计划帧回归环境专用动作。计划能先生成稀疏关键帧再细化，也可在采样时施加额外约束。原文在组合泛化、多任务与层级规划上评估，并探索互联网视频知识迁移。

带着这个问题读：先生成机器人会怎么做的视频，再倒推出动作，这条路线解决了什么又把难题搬到了哪里？

初读判断：NeurIPS PDF 定义统一预测决策过程、视频到动作接口和分层采样，并分别评估组合与跨任务能力；控制与可见视频计划要分层看，实机证据评分较谨慎。

## 七维评分

![七维雷达：加载时展开一次，随后静止](radar.gif)

打开时从中心展开一次，结束后保持最终形状。[直接查看静态图](radar.svg)。加载与再次打开的播放时机取决于浏览器缓存。

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 刊会质量 | 95.0 | 30% |
| 创新性 | 93 | 20% |
| 实验与证据 | 86 | 20% |
| 学术影响 | 33.8 | 10% |
| 近期关注 | 42.5 | 5% |
| 复用价值 | 80 | 8% |
| 阅读价值 | 96 | 7% |

刊会依据：[NeurIPS 2023](../../../venues/NeurIPS/README.md)，正式出处见[出版/原文记录](https://proceedings.neurips.cc/paper_files/paper/2023/hash/1d5b9233ad716a43be5c0d3023cb82d0-Abstract-Conference.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：正式刊会版本；OpenAlex题目：Learning Universal Policies via Text-Guided Video Generation。累计被引 14，2025–2026 被引 13；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W7133231380) · [文献计量条目](https://openalex.org/W7133231380)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
