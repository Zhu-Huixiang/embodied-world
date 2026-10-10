# Octo: An Open-Source Generalist Robot Policy

本版阅读优先顺序：36；综合分：88.3 / 100；已评分权重：100%。

[原文](https://www.roboticsproceedings.org/rss20/p090.html) · [PDF](https://roboticsproceedings.org/rss20/p090.pdf) · [阅读卡片](../../../library/octo.md)

## 机制简析

各类任务、图像和本体感觉先由模态 tokenizer 转成 token，Transformer 主干处理后由读取头和扩散解码器产生动作块。更换机器人时，输入或输出适配器可改变，而主干保留预训练知识并微调。项目在不同平台上区分零样本运行与小数据微调，还单独检验新力传感输入和关节控制空间。

带着这个问题读：通用策略接上新摄像头、新动作空间时，哪些模块可以保留，哪些需要改？

初读判断：RSS 论文与项目给出九个平台的评估、结构和数据消融、完整开放训练及微调资源；方法创新主要在可扩展接口和组合设计，证据与复用价值突出。

## 七维评分

![七维雷达：加载时展开一次，随后静止](radar.gif)

打开时从中心展开一次，结束后保持最终形状。[直接查看静态图](radar.svg)。加载与再次打开的播放时机取决于浏览器缓存。

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 刊会质量 | 95.0 | 30% |
| 创新性 | 87 | 20% |
| 实验与证据 | 91 | 20% |
| 学术影响 | 59.2 | 10% |
| 近期关注 | 75.8 | 5% |
| 复用价值 | 99 | 8% |
| 阅读价值 | 94 | 7% |

刊会依据：[RSS 2024](../../../venues/RSS/README.md)，正式出处见[出版/原文记录](https://www.roboticsproceedings.org/rss20/p090.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：Octo: An Open-Source Generalist Robot Policy。累计被引 113，2025–2026 被引 110；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4402353985) · [文献计量条目](https://openalex.org/W4402353985)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
