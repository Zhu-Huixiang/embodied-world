# PaLM-E: An Embodied Multimodal Language Model

**解读导读** · ICML 2023 · [视觉语言动作模型 VLA](../paper-map/README.md#track-vla)

研究范围：连续感知到语言空间的具身多模态推理与高层操作规划。

[原文入口](https://proceedings.mlr.press/v202/driess23a.html) · [原文 PDF](https://proceedings.mlr.press/v202/driess23a/driess23a.pdf) · [作者项目 / 代码入口](https://palm-e.github.io/)

收录 ICML 2023 正式版。PaLM-E 产生文字计划，勿混写成 RT-2 式直接动作 token 策略。

## 先看它做了什么

视觉和连续状态由编码器变成与语言 token 等维的向量，和文本交错组成多模态句子，再交给 decoder-only 语言模型生成文字。训练同时覆盖机器人任务、视觉问答和图文任务，以检验知识是否产生正迁移。机器人演示中，文字计划交给底层策略执行，后续视觉反馈再进入模型。

## 带着什么问题读

**把传感器读数塞进语言模型的 embedding 空间，能带来怎样的机器人推理？**

## 为什么值得继续读

具身多模态语言模型的标志性论文，清楚连接感知接入、互联网知识迁移与机器人规划。

证据入口：ICML 原文与项目页包含多种输入模态、多个具身平台、跨任务联合训练及规模研究；完整大模型未提供可直接复现实验的开放训练资源，因此复用分低于 Octo。

具身关联：具身多模态语言模型的标志性论文，清楚连接感知接入、互联网知识迁移与机器人规划。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/palm-e/README.md) · [ICML集锦](../venues/ICML/README.md) · [地图方向](../paper-map/README.md#track-vla) · [首页](../README.md)

元数据核对：2026-10-10。
