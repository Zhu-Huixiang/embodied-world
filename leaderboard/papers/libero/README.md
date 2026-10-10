# LIBERO: Benchmarking Knowledge Transfer for Lifelong Robot Learning

**LIBERO** · NeurIPS 2023 · 本版排名 34 · 综合分 **88.7 / 100**

[解读导读](../../../library/libero.md) · [操作与动作块](../../../paper-map/README.md#track-manipulation) · [NeurIPS集锦](../../../venues/NeurIPS/README.md)

[原文](https://proceedings.neurips.cc/paper_files/paper/2023/hash/8c3c666820ea055a77726d66fc7d447f-Abstract.html) · [PDF](https://proceedings.neurips.cc/paper_files/paper/2023/file/8c3c666820ea055a77726d66fc7d447f-Paper-Datasets_and_Benchmarks.pdf) · [阅读卡片](../../../library/libero.md)

## 机制简析

程序化构造物体、空间、目标和长任务不同组合，把迁移对象拆成概念知识与执行知识；模型按任务顺序学习，在新任务上只能有限访问旧数据。评测分别检查前向迁移、遗忘、任务顺序和预训练作用。原文比较顺序微调、回放和保留参数等办法，发现某些防遗忘方法会压制新任务学习。

带着这个问题读：一个机器人顺序学新任务时，究竟迁移的是物体概念、动作技能，还是两者的组合？

初读判断：NeurIPS 正式 PDF 给出四套任务、人类示范、架构/终身算法/顺序/预训练研究，复用广且评测设计有清楚科学问题；不能只把它理解成榜单分母。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 88 | 20% |
| 实验与证据 | 93 | 20% |
| 学术影响 | 57.9 | 10% |
| 近期关注 | 74.6 | 5% |
| 复用价值 | 99 | 8% |
| 阅读价值 | 94 | 7% |

刊会依据：[NeurIPS 2023](../../../venues/NeurIPS/README.md)，正式出处见[出版/原文记录](https://proceedings.neurips.cc/paper_files/paper/2023/hash/8c3c666820ea055a77726d66fc7d447f-Abstract.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：正式刊会版本；OpenAlex题目：LIBERO: Benchmarking Knowledge Transfer for Lifelong Robot Learning。累计被引 102，2025–2026 被引 102；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W7133220882) · [文献计量条目](https://openalex.org/W7133220882)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
