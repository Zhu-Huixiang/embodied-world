# Diffusion Forcing: Next-token Prediction Meets Full-sequence Diffusion

**Diffusion Forcing** · NeurIPS 2024 · 本版排名 47 · 综合分 **86.3 / 100**

[解读导读](../../../library/diffusion-forcing.md) · [视频与序列生成](../../../paper-map/README.md#track-video-generation) · [NeurIPS集锦](../../../venues/NeurIPS/README.md)

[原文](https://proceedings.neurips.cc/paper_files/paper/2024/hash/2aee1c4159e48407d68fe16ae8e6e49e-Abstract-Conference.html) · [PDF](https://proceedings.neurips.cc/paper_files/paper/2024/file/2aee1c4159e48407d68fe16ae8e6e49e-Paper-Conference.pdf) · [阅读卡片](../../../library/diffusion-forcing.md)

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
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 95 | 20% |
| 实验与证据 | 86 | 20% |
| 学术影响 | 49.1 | 10% |
| 近期关注 | 63.2 | 5% |
| 复用价值 | 90 | 8% |
| 阅读价值 | 91 | 7% |

刊会依据：[NeurIPS 2024](../../../venues/NeurIPS/README.md)，正式出处见[出版/原文记录](https://proceedings.neurips.cc/paper_files/paper/2024/hash/2aee1c4159e48407d68fe16ae8e6e49e-Abstract-Conference.html)；采用2026-10-10刊会快照。


编辑深度：选题初读；评分记录：2026-10-10。

计量版本：正式刊会版本；OpenAlex题目：Diffusion Forcing: Next-token Prediction Meets Full-Sequence Diffusion。累计被引 50，2025–2026 被引 50；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W4415798523) · [文献计量条目](https://openalex.org/W4415798523)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
