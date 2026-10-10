# Octo: An Open-Source Generalist Robot Policy

**解读导读** · RSS 2024 · [视觉语言动作模型 VLA](../paper-map/README.md#track-vla)

研究范围：跨机器人通用策略、扩散动作头与可适配多模态接口。

[原文入口](https://www.roboticsproceedings.org/rss20/p090.html) · [原文 PDF](https://roboticsproceedings.org/rss20/p090.pdf) · [作者项目 / 代码入口](https://octo-models.github.io/)

以 RSS 2024 版本为准；预训练数据、模型大小与微调数据不混为同一实验条件。

## 先看它做了什么

各类任务、图像和本体感觉先由模态 tokenizer 转成 token，Transformer 主干处理后由读取头和扩散解码器产生动作块。更换机器人时，输入或输出适配器可改变，而主干保留预训练知识并微调。项目在不同平台上区分零样本运行与小数据微调，还单独检验新力传感输入和关节控制空间。

## 带着什么问题读

**通用策略接上新摄像头、新动作空间时，哪些模块可以保留，哪些需要改？**

## 为什么值得继续读

公开通用机器人策略与复用训练接口的重要基线，完整开放模型、预训练/微调代码和数据加载器。

证据入口：RSS 论文与项目给出九个平台的评估、结构和数据消融、完整开放训练及微调资源；方法创新主要在可扩展接口和组合设计，证据与复用价值突出。

具身关联：公开通用机器人策略与复用训练接口的重要基线，完整开放模型、预训练/微调代码和数据加载器。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/octo/README.md) · [RSS集锦](../venues/RSS/README.md) · [地图方向](../paper-map/README.md#track-vla) · [首页](../README.md)

元数据核对：2026-10-10。
