# VioLA: Learning Generalist Humanoid Control Policies from Human Data

**解读导读** · arXiv 2026 · [视觉语言动作模型 VLA](../paper-map/README.md#track-vla)

研究范围：机器人学习。

[原文入口](https://arxiv.org/abs/2610.12435v1) · [原文 PDF](https://arxiv.org/pdf/2610.12435v1) · [作者项目 / 代码入口](https://viola.is.tue.mpg.de)

## 先看它做了什么

VLA 预测身体与手部运动 latent，预训练控制器负责执行；运动编码器把人类示范映射到同一空间，扩大可监督动作池。

## 带着什么问题读

**人类动作怎样先对齐控制器，再教会人形 VLA？**

## 为什么值得继续读

跨数据监督和动作空间转换直接对上 Holo-M；初读关注零样本协议、控制器预训练与总数据规模。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/viola/README.md) · [arXiv集锦](../arxiv/README.md#paper-viola) · [地图方向](../paper-map/README.md#track-vla) · [首页](../README.md)

元数据核对：2026-10-09T18:35:28+08:00。
