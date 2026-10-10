# VIMA: Robot Manipulation with Multimodal Prompts

**解读导读** · ICML 2023 · [视觉语言动作模型 VLA](../paper-map/README.md#track-vla)

研究范围：多模态提示、桌面操作与系统化组合泛化评测。

[原文入口](https://proceedings.mlr.press/v202/jiang23b.html) · [原文 PDF](https://proceedings.mlr.press/v202/jiang23b/jiang23b.pdf) · [作者项目 / 代码入口](https://vimalabs.github.io/)

ICML 2023 正式版；VIMA-Bench 是仿真桌面任务，勿把仿真规模当实机证据。

## 先看它做了什么

对象图像 token 与文字交错构成任务提示，再经 T5 编码；因果 Transformer 通过交叉注意力读取提示，并结合交互历史自回归输出动作。程序化生成任务按不同泛化难度拆开测试，避免只看训练分布平均成功率。原文对对象 tokenizer、提示接入方式、模型规模和数据量分别消融。

## 带着什么问题读

**文字、目标图和示范视频能否作为同一种任务提示交给机器人？**

## 为什么值得继续读

把不同机器人任务描述统一为多模态 prompt 的重要工作，配套系统泛化协议和架构消融。

证据入口：ICML 正式版与项目给出四级泛化协议、数据/规模研究和对象 token 消融，公开基准便于后续方法比较；实机证据弱于 RT-1，证据评分体现这一点。

具身关联：把不同机器人任务描述统一为多模态 prompt 的重要工作，配套系统泛化协议和架构消融。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/vima/README.md) · [ICML集锦](../venues/ICML/README.md) · [地图方向](../paper-map/README.md#track-vla) · [首页](../README.md)

元数据核对：2026-10-10。
