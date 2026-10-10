# LIBERO: Benchmarking Knowledge Transfer for Lifelong Robot Learning

**LIBERO** · NeurIPS 2023 · 本版排名 28 · 综合分 **89.6 / 100**

[解读导读](../../../library/libero.md) · [操作与动作块](../../../paper-map/README.md#track-manipulation) · [NeurIPS集锦](../../../venues/NeurIPS/README.md)

[原文](https://proceedings.neurips.cc/paper_files/paper/2023/hash/8c3c666820ea055a77726d66fc7d447f-Abstract.html) · [PDF](https://proceedings.neurips.cc/paper_files/paper/2023/file/8c3c666820ea055a77726d66fc7d447f-Paper-Datasets_and_Benchmarks.pdf) · [阅读卡片](../../../library/libero.md)

论文出处：[Bo Liu / Yifeng Zhu 等3位 · UT Austin Robot Perception and Learning Lab（RPL） / The University of Texas at Austin 等4个出处](../../origins/papers/libero.md)

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
| 公开与评审 | 95.0 | 30% |
| 创新性 | 88 | 20% |
| 实验与证据 | 93 | 20% |
| 学术影响 | 57.9 | 10% |
| 近期关注 | 91.7 | 5% |
| 复用价值 | 99 | 8% |
| 阅读价值 | 94 | 7% |

刊会依据：[NeurIPS 2023](../../../venues/NeurIPS/README.md)，正式出处见[出版/原文记录](https://proceedings.neurips.cc/paper_files/paper/2023/hash/8c3c666820ea055a77726d66fc7d447f-Abstract.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：LIBERO: Benchmarking Knowledge Transfer for Lifelong Robot Learning。累计被引 **102**，2025–2026 被引 **102**；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W7133220882) · [文献计量条目](https://openalex.org/W7133220882)

### 影响与关注的计算依据

- **学术影响 57.9**：身份匹配的累计引用C=102，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W7133220882)
- **近期关注 91.7**：huggingface 的论文专属入口：HF 最近30天下载=38432；按100000上限对数压缩。 [依据1](https://huggingface.co/api/datasets/physical-intelligence/libero) · [依据2](https://huggingface.co/datasets/physical-intelligence/libero/raw/main/README.md) · [依据3](https://huggingface.co/datasets/physical-intelligence/libero)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/Lifelong-Robot-Learning/LIBERO) | GitHub Star 2404；GitHub Watch订阅 8；GitHub Fork 510 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/datasets/physical-intelligence/libero) | HF 最近30天下载 38432；HF 仓库累计点赞 93 | 单篇论文的第三方实现/数据格式转换，按此仓库统计；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2306.03310) | HF 论文累计点赞 3 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
