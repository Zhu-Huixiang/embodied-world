# Self Forcing: Bridging the Train-Test Gap in Autoregressive Video Diffusion

**解读导读** · NeurIPS 2025 · [视频与序列生成](../paper-map/README.md#track-video-generation)

研究范围：视频生成基础；机器人部署另看策略论文。

[原文入口](https://proceedings.neurips.cc/paper_files/paper/2025/hash/f4823f831af67a3ef15e41a85434422a-Abstract-Conference.html) · [原文 PDF](https://proceedings.neurips.cc/paper_files/paper/2025/file/f4823f831af67a3ef15e41a85434422a-Paper-Conference.pdf)

## 先看它做了什么

使用模型自己的历史滚动来训练自回归视频生成，减少教师历史与部署历史的分布差异。

## 带着什么问题读

**用模型自己滚出的历史训练，怎样处理自回归误差累积？**

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/self-forcing/README.md) · [NeurIPS集锦](../venues/NeurIPS/README.md) · [地图方向](../paper-map/README.md#track-video-generation) · [首页](../README.md)

元数据核对：2026-10-09。
