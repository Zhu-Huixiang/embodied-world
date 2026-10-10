# Diffusion Forcing: Next-token Prediction Meets Full-sequence Diffusion

**Diffusion Forcing** · NeurIPS 2024 · 本版排名 50 · 综合分 **85.5 / 100**

[解读导读](../../../library/diffusion-forcing.md) · [视频与序列生成](../../../paper-map/README.md#track-video-generation) · [NeurIPS集锦](../../../venues/NeurIPS/README.md)

[原文](https://proceedings.neurips.cc/paper_files/paper/2024/hash/2aee1c4159e48407d68fe16ae8e6e49e-Abstract-Conference.html) · [PDF](https://proceedings.neurips.cc/paper_files/paper/2024/file/2aee1c4159e48407d68fe16ae8e6e49e-Paper-Conference.pdf) · [阅读卡片](../../../library/diffusion-forcing.md)

论文出处：[Boyuan Chen · MIT / MIT CSAIL 等3个出处](../../origins/papers/diffusion-forcing.md)

## 机制简析

让序列各位置带不同噪声等级，把下一步预测与整段扩散连接，支持因果生成和引导。

带着这个问题读：各时间步不同噪声强度，怎样连接因果预测与整序列去噪？

初读判断：噪声安排与时序条件具有方法创新；机器人用途需看具体规划实验。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 95 | 20% |
| 实验与证据 | 86 | 20% |
| 学术影响 | 49.1 | 10% |
| 近期关注 | 47.0 | 5% |
| 复用价值 | 90 | 8% |
| 阅读价值 | 91 | 7% |

刊会依据：[NeurIPS 2024](../../../venues/NeurIPS/README.md)，正式出处见[出版/原文记录](https://proceedings.neurips.cc/paper_files/paper/2024/hash/2aee1c4159e48407d68fe16ae8e6e49e-Abstract-Conference.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：选题初读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：Diffusion Forcing: Next-token Prediction Meets Full-Sequence Diffusion。累计被引 **50**，2025–2026 被引 **50**；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W4415798523) · [文献计量条目](https://openalex.org/W4415798523)

### 影响与关注的计算依据

- **学术影响 49.1**：身份匹配的累计引用C=50，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4415798523)
- **近期关注 47.0**：近期已定位引用R=50；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W4415798523)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [huggingface](https://huggingface.co/papers/2407.01392) | HF 论文累计点赞 43 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
