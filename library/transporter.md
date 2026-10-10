# Transporter Networks: Rearranging the Visual World for Robotic Manipulation

**解读导读** · CoRL 2020 · [操作与动作块](../paper-map/README.md#track-manipulation)

研究范围：空间等变、拾取条件放置与 Ravens 操作基准。

[原文入口](https://proceedings.mlr.press/v155/zeng21a.html) · [原文 PDF](https://proceedings.mlr.press/v155/zeng21a/zeng21a.pdf) · [作者项目 / 代码入口](https://transporternets.github.io/)

CoRL 2020，PMLR 155 于 2021-10-04 出版，均早于窗口；明确作为经典基础例外收录。

## 先看它做了什么

网络先在 RGB-D 视觉空间中预测拾取区域，取出局部深层特征，再将它与整幅场景特征互相关来确定放置位置和旋转。动作输出与输入空间对应，平移和旋转结构被模型直接利用，不先构建对象姿态或分割。原文覆盖刚体、绳索和堆物推动，比较样本效率，并扩展到六自由度拾放和真实机器人。

## 带着什么问题读

**操作物体不一定要先识别物体？空间特征之间的匹配怎么直接长出动作？**

## 为什么值得继续读

CLIPort 等空间操作路线的直接基础，把动作对齐到视觉空间并利用平移/旋转对称性，具有持续方法影响和开放基准价值。

证据入口：CoRL 正式版给出多种操作任务和真实验证，作者开放 Ravens、数据、模型及代码；CLIPort 原文和项目明确继承这一机制，可追溯的路线影响足以支持年限例外。

具身关联：CLIPort 等空间操作路线的直接基础，把动作对齐到视觉空间并利用平移/旋转对称性，具有持续方法影响和开放基准价值。

经典保留理由：早于五年窗口的经典基础；CLIPort 直接使用其拾取/放置网络，Ravens 基准与动作中心空间归纳偏置持续影响后续操作研究。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/transporter/README.md) · [CoRL集锦](../venues/CoRL/README.md) · [地图方向](../paper-map/README.md#track-manipulation) · [首页](../README.md)

元数据核对：2026-10-10。
