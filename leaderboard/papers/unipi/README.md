# Learning Universal Policies via Text-Guided Video Generation

**UniPi** · NeurIPS 2023 · 本版排名 85 · 综合分 **82.2 / 100**

[解读导读](../../../library/unipi.md) · [视频动作模型与视觉推理](../../../paper-map/README.md#track-video-action) · [NeurIPS集锦](../../../venues/NeurIPS/README.md)

[原文](https://proceedings.neurips.cc/paper_files/paper/2023/hash/1d5b9233ad716a43be5c0d3023cb82d0-Abstract-Conference.html) · [PDF](https://proceedings.neurips.cc/paper_files/paper/2023/file/1d5b9233ad716a43be5c0d3023cb82d0-Paper-Conference.pdf) · [阅读卡片](../../../library/unipi.md)

论文出处：[Yilun Du · MIT / Google DeepMind 等5个出处](../../origins/papers/unipi.md)

## 机制简析

当前图像和文字任务条件送入视频扩散模型，生成未来画面序列作为计划；逆动力学模型再从相邻或计划帧回归环境专用动作。计划能先生成稀疏关键帧再细化，也可在采样时施加额外约束。原文在组合泛化、多任务与层级规划上评估，并探索互联网视频知识迁移。

带着这个问题读：先生成机器人会怎么做的视频，再倒推出动作，这条路线解决了什么又把难题搬到了哪里？

初读判断：NeurIPS PDF 定义统一预测决策过程、视频到动作接口和分层采样，并分别评估组合与跨任务能力；控制与可见视频计划要分层看，实机证据评分较谨慎。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 93 | 20% |
| 实验与证据 | 86 | 20% |
| 学术影响 | 33.8 | 10% |
| 近期关注 | 27.3 | 5% |
| 复用价值 | 80 | 8% |
| 阅读价值 | 96 | 7% |

刊会依据：[NeurIPS 2023](../../../venues/NeurIPS/README.md)，正式出处见[出版/原文记录](https://proceedings.neurips.cc/paper_files/paper/2023/hash/1d5b9233ad716a43be5c0d3023cb82d0-Abstract-Conference.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：Learning Universal Policies via Text-Guided Video Generation。累计被引 **14**，2025–2026 被引 **13**；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W7133231380) · [文献计量条目](https://openalex.org/W7133231380)

### 影响与关注的计算依据

- **学术影响 33.8**：身份匹配的累计引用C=14，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W7133231380)
- **近期关注 27.3**：近期已定位引用R=13；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W7133231380)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [huggingface](https://huggingface.co/papers/2302.00111) | HF 论文累计点赞 0 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
