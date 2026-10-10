# VIMA: Robot Manipulation with Multimodal Prompts

**VIMA** · ICML 2023 · 本版排名 52 · 综合分 **85.8 / 100**

[原文](https://proceedings.mlr.press/v202/jiang23b.html) · [PDF](https://proceedings.mlr.press/v202/jiang23b/jiang23b.pdf) · [阅读卡片](../../../library/vima.md)

## 机制简析

对象图像 token 与文字交错构成任务提示，再经 T5 编码；因果 Transformer 通过交叉注意力读取提示，并结合交互历史自回归输出动作。程序化生成任务按不同泛化难度拆开测试，避免只看训练分布平均成功率。原文对对象 tokenizer、提示接入方式、模型规模和数据量分别消融。

带着这个问题读：文字、目标图和示范视频能否作为同一种任务提示交给机器人？

初读判断：ICML 正式版与项目给出四级泛化协议、数据/规模研究和对象 token 消融，公开基准便于后续方法比较；实机证据弱于 RT-1，证据评分体现这一点。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 91 | 20% |
| 实验与证据 | 89 | 20% |
| 学术影响 | 52.1 | 10% |
| 近期关注 | 45.6 | 5% |
| 复用价值 | 92 | 8% |
| 阅读价值 | 92 | 7% |

刊会依据：[ICML 2023](../../../venues/ICML/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v202/jiang23b.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：VIMA: General Robot Manipulation with Multimodal Prompts。累计被引 64，2025–2026 被引 16；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4303648971) · [文献计量条目](https://openalex.org/W4303648971)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
